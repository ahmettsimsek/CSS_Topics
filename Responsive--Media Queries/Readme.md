🎯 Proje Amacı

Responsive tasarım mantığını öğrenmek

@media kullanımını anlamak

display: none ve display: block farkını görmek

vw birimi ile dinamik font boyutu ayarlamak

Görselleri responsive yapmak

🖥️ Ekran Boyutlarına Göre Davranış

Sayfa açıldığında tüm <h1> etiketleri gizlidir:

```
   h1 {
  display: none;
}
```

Ekran genişliğine göre yalnızca ilgili başlık görünür

Ekran Türü	Genişlik Aralığı	Gösterilen Başlık
📱 Mobile	320px – 480px	mobile
📱 Tablet	481px – 768px	tablets
💻 Laptop	769px – 1024px	laptops
🖥️ Desktop	1025px – 1200px	desktop
🖥️ Large Screen	1201px+	large screen
🖼️ Responsive Image

```
img {
  max-width: 100%;
  height: auto;
}
```

Bu sayede:

Görsel ekran genişliğini aşmaz

Oranı bozulmaz

Küçük ekranlarda taşma yapmaz

🔤 VW ile Font Boyutlandırma
```
p {
  font-size: 10vw;
}
```

vw = viewport width

1vw = ekran genişliğinin %1’i

Font boyutu ekran genişliğine göre otomatik büyür/küçülür

🚀 Kullanılan Teknolojiler

HTML5

CSS3

Media Queries

Responsive Design

📌 Öğrenilen Konular

Responsive Web Design

CSS Breakpoints

Display Property

Viewport Units (vw)

Image Scaling Techniques

▶️ Nasıl Çalıştırılır?

Dosyayı indirin

index.html dosyasını tarayıcıda açın

Tarayıcıyı küçültüp büyüterek responsive davranışı gözlemleyin

📷 Demo

Tarayıcı boyutunu değiştirerek farklı ekran türlerinin nasıl göründüğünü test edebilirsiniz.
