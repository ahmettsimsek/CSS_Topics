🎨 CSS Transition & Animation Lab
Bu proje, HTML öğeleri üzerinde CSS geçiş efektlerinin (transitions) nasıl çalıştığını, zamanlama fonksiyonlarının farklarını ve gelişmiş animasyon tekniklerini görselleştirmek için hazırlanmış bir eğitim setidir.

🚀 Proje Özeti
Proje, 13 farklı kutu (.box - .box13) üzerinden CSS'in dinamik özelliklerini test eder. Her kutu, farklı bir transition-timing-function veya property (özellik) kombinasyonunu temsil eder.

🛠 Teknik İçerik
1. Zamanlama Fonksiyonları (Timing Functions)
Animasyonun hız eğrisini belirleyen temel fonksiyonlar karşılaştırmalı olarak uygulanmıştır:

ease: Yavaş başlar, ortada hızlanır ve yavaş biter.

ease-in: Yavaş başlar, sona doğru ivme kazanır.

ease-out: Hızlı başlar, sona doğru yavaşlar (Yumuşak duruş).

ease-in-out: Hem başlangıç hem bitiş yavaştır; en doğal görünümü sağlar.

linear: Sabit hızda ilerler.

steps(n): Animasyonu akıcı değil, belirlenen adım sayısında (kesik kesik) oynatır.

cubic-bezier: Dört kontrol noktası ile tamamen özel hız eğrileri oluşturur.

2. Dönüşüm ve Ölçekleme (Transform & Scale)
Sadece genişlik/yükseklik değil, öğenin fiziksel yapısını değiştiren özellikler kullanılmıştır:
```
rotate(135deg): Öğeyi 135 derece döndürür.
```
```
scale(2): Öğeyi orijinal boyutunun 2 katına çıkarır.
```
```
transform-property: Animasyonun hangi fiziksel değişime odaklanacağını seçer.
```
📦 Kod Yapısı ve Kullanım
Tekli vs. Çoklu Tanımlama
Projede hem uzun yazım (Longhand) hem de kısa yazım (Shorthand) teknikleri gösterilmiştir:

Çoklu Geçiş Örneği (.box12):
```
CSS
transition: transform 1s ease 0s, 
            background-color 3s ease 0s, 
            scale 3s ease;
Kısayol (Shorthand) Kullanımı (.box13):
```
```
CSS
/* Mülk | Süre | Zamanlama | Gecikme */
transition: all 1s ease-in-out 0s;
```
