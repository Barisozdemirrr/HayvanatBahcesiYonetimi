# Hayvanat Bahçesi Yönetimi - UML Sınıf Diyagramı

Bu proje, polimorfizm prensibi temel alınarak hazırlanmış bir hayvanat bahçesi yönetim sistemine ait UML sınıf diyagramı tasarımı içermektedir. Amaç; nesne yönelimli programlamanın temel kavramlarının (kalıtım, polimorfizm, soyutlama) gerçek bir senaryo üzerinde uygulanmasını modellemektir.

## Proje Hakkında

Hayvanat bahçesindeki farklı hayvan türlerinin (memeli, kuş, sürüngen, balık vb.) ortak ve özel davranışları nesne yönelimli yaklaşımla modellenmiştir. Tasarım `Hayvanat Bahcesi.drawio.png` görselinde sunulan sınıf diyagramı üzerinden açıklanmaktadır.

### Modellenen Kavramlar

- **Soyut sınıf (Abstract Class)**: Ortak özelliklerin (isim, yaş, ses çıkarma vb.) üst sınıfta toplanması
- **Kalıtım (Inheritance)**: Türlere özgü hayvan sınıflarının üst sınıftan türetilmesi
- **Polimorfizm (Polymorphism)**: Aynı metodun farklı hayvan türlerinde farklı davranış sergilemesi
- **Encapsulation**: Hayvan özelliklerinin private alanlar ile korunması
- **Aggregation**: Hayvanat bahçesi ile hayvanlar arasındaki "sahip olma" ilişkisi

## Kullanılan Java Konseptleri (Tasarımda Önerilen)

Bu proje bir kod tabanı yerine bir **tasarım dokümantasyonu** niteliğindedir. Diyagramda kullanılan ve Java diline aktarılabilecek özellikler şunlardır:

- **OOP**: Encapsulation, Inheritance, Polymorphism, Abstraction
- **Abstract Class & Method**: Hayvan üst sınıfı ve tür-özgü `sesCikar()` benzeri soyut metotlar
- **Interface**: Beslenme, hareket gibi davranışların arayüzler ile ayrıştırılması
- **Collections**: Hayvanat bahçesindeki hayvan listesinin `List<Animal>` ile yönetilmesi
- **UML**: Class Diagram notasyonu

## Proje İçeriği

```
HayvanatBahcesiYonetimi/
├── Hayvanat Bahcesi.drawio.png   (UML Sınıf Diyagramı)
└── README.md
```

## Diyagramı Görüntüleme

`Hayvanat Bahcesi.drawio.png` dosyasını herhangi bir görsel görüntüleyici ile açabilirsiniz. Diyagramı düzenlemek için [draw.io](https://app.diagrams.net) (eski adıyla diagrams.net) platformunu kullanabilirsiniz.

## Diyagramı Java'ya Aktarma

Tasarımı kod düzeyinde uygulamak için aşağıdaki gibi bir paket yapısı önerilir:

```
src/
├── Animal.java            (abstract)
├── Mammal.java            (extends Animal)
├── Bird.java              (extends Animal)
├── Reptile.java           (extends Animal)
├── Feedable.java          (interface)
└── Zoo.java               (List<Animal>)
```

## Notlar

> Bu repo, hayvanat bahçesi yönetimi konseptinin sınıf diyagramı üzerinden anlatımına odaklanmaktadır. Java implementasyonu kullanıcı tarafından gerçekleştirilmek üzere referans olarak hazırlanmıştır.
