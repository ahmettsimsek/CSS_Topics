#🚀 CSS Animasyonları ve Konumlandırma (Position) Çalışması
Bu proje, CSS kullanarak öğeleri nasıl hareket ettirebileceğimizi, renk geçişlerini nasıl yöneteceğimizi ve position özelliklerinin mantığını anlamak için hazırlanmış bir uygulama rehberidir.

## 🛠 Öğrenilen Teknik Özellikler
## 1. CSS Animasyon Temelleri
Animasyonları tanımlamak için @keyframes yapısını ve bu animasyonları tetiklemek için kullanılan temel parametreleri inceledik:

animation-duration: Hareketin ne kadar süreceği (Örn: 4s).

animation-delay: Başlamadan önceki bekleme süresi.

animation-iteration-count: Tekrar sayısı (infinite ile sonsuz döngü).

animation-direction: Hareketin yönü (alternate ile git-gel yapma).

animation-fill-mode: Animasyon bitince öğenin nerede duracağı (forwards ile sonda kalma).

## 2. Boşluk Yönetimi (Box Model)
Margin: Öğeler arası dış boşluk bırakmak için kullanıldı. Özellikle kutuların alt alta yapışmaması için margin-top ve margin-bottom tercih edildi.

## 3. Konumlandırma Mantığı (Positioning)
Position: Relative: Öğeyi normal akıştan koparmadan, kendi orijinal yerine göre hareket ettirmemizi sağlar.

Position: Absolute: Öğeyi bağımsız bir katmana çıkarır ve en yakın relative atasına göre konumlandırır.

## 📦 Proje İçeriği ve Deneyler
```
Öğe,Yapılan İşlem,Kullanılan Özellik
1. Kutu,Basit Renk Geçişi,from - to Keyframes
2. Kutu,Çoklu Renk Geçişi,% (Yüzdelik) Keyframes
3. Kutu,Kare Çizerek Hareket,"left, top ve alternate"
4. Kutu,Başa Dönme,fill-mode: backwards
5. Kutu,Sonda Sabit Kalma,fill-mode: forwards
```
