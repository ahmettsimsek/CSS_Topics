# 🚀 3D Animated Navigation Menu
Bu proje, CSS'in ::before ve ::after sözde öğeleri (pseudo-elements) ve 3D transform özellikleri kullanılarak hazırlanmış, interaktif bir navigasyon menüsüdür. Fare ile üzerine gelindiğinde (hover), menü elemanları üç boyutlu bir kapak açılma efektiyle renk ve içerik değiştirir.

## ✨ Özellikler
3D Dönüşümler: rotateX kullanılarak oluşturulan derinlik algısı.

Gecikmeli Animasyon: Üst ve alt kapakların (before & after) ardışık açılması için transition-delay kullanımı.

Dinamik İçerik: CSS attr(data-text) özelliği sayesinde HTML'deki verinin otomatik olarak animasyon katmanlarına taşınması.

Tam Hizalama: Flexbox kullanılarak sayfa ortasında mükemmel konumlandırma.

## 🛠️ Kullanılan Teknolojiler
HTML5: Yapısal iskelet ve data-* nitelikleri.

CSS3: * Position: Absolute/Relative (Konumlandırma)

Transform-origin (Menteşe etkisi oluşturma)

Transition (Geçiş efektleri)

Pseudo-elements (::before, ::after)

## 📖 Teknik Detaylar
1. Menteşe Mantığı (transform-origin)
Menü elemanlarının bir kapı veya kapak gibi açılmasını sağlamak için dönüş noktaları sabitlenmiştir:

Üst Kapak: transform-origin: top; ile üst kenardan döner.

Alt Kapak: transform-origin: bottom; ile alt kenardan döner.

2. Ardışık Efekt (transition-delay)
Kapakların aynı anda değil, birbiri ardına açılması için ikinci katmana (after) 300ms gecikme eklenmiştir. Bu, animasyona daha akıcı ve mekanik bir his katar.
```
CSS
nav ul li a:hover::after {
    transition-delay: 300ms;
    transform: rotateX(0deg);
}
```
3. Veri Çekme (data-text)
HTML tarafında tanımlanan data-text niteliği, CSS tarafında content: attr(data-text); komutuyla okunur. Bu sayede her link için ayrı CSS yazmaya gerek kalmaz, kod kendini tekrar etmez.
