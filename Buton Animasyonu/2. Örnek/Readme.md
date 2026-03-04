# 🚀 Modern CSS Button Hover Animations

Bu proje, HTML ve CSS kullanarak oluşturulmuş, kullanıcı etkileşimini ön plana çıkaran modern buton animasyonlarını içerir. Projede özellikle **CSS Pseudo-elements (`::before`)** ve **Transform** yetenekleri kullanılarak "katmanlı dolgu" efektleri üzerinde durulmuştur.

## ✨ Öne Çıkan Özellikler

- **Pürüzsüz Geçişler:** `transition` özelliği ile tüm renk ve boyut değişimleri akıcı hale getirilmiştir.
- **Yaylanma Efekti (Bounce):** `cubic-bezier(0.5, 1.6, 0.4, 0.7)` hız eğrisi kullanılarak buton dolgusuna doğal bir esneklik kazandırılmıştır.
- **Donanım Hızlandırmalı Performans:** Animasyonlar `width/height` yerine `transform: scale()` ile yapıldığı için tarayıcıda kasma yapmadan (60fps) çalışır.
- **Kusursuz Merkezleme:** Flexbox yerine klasik `absolute` + `translate` yöntemiyle her ekran boyutunda tam merkezleme sağlanmıştır.

---

## 🛠️ Teknik Detaylar ve Mantık

### 1. Katmanlama (Z-Index) Stratejisi
Butonun içindeki metnin, arkadan gelen dolgu renginin altında kalmaması için şu hiyerarşi izlenmiştir:
- `.btn`: `z-index: 1` (Yazı katmanı)
- `.btn::before`: `z-index: -1` (Arka plandaki renk katmanı)

### 2. Maskeleme (Overflow)
Dolgu rengi butonun dışına taşmasın diye `.btn` sınıfına `overflow: hidden;` eklenmiştir. Bu, animasyonun sadece butonun sınırları içinde görünmesini sağlar.

[Image of CSS overflow hidden visualization]

### 3. Animasyon Tipleri

| Sınıf | Teknik | Açıklama |
| :--- | :--- | :--- |
| `.btn1` | `scaleX(0)` → `scaleX(1)` | Sol üst köşeden (`0 0`) başlayarak sağa doğru yatay dolgu. |
| `.btn2` | `scaleY(0)` → `scaleY(1)` | Sol üst köşeden (`0 0`) başlayarak aşağı doğru dikey dolgu. |

[Image of CSS transform scaleX vs scaleY visualization]

---

## 📦 Kodun Anatomisi

Projede kullanılan en kritik CSS bloğu:

```css
.btn::before {
    content: "";              /* Sanal elemanı oluşturur */
    position: absolute;       /* Butona göre sabitler */
    transition: transform 0.5s; /* Hareket süresi */
    transform-origin: 0 0;    /* Animasyonun başlangıç noktası (Sol Üst) */
    transition-timing-function: cubic-bezier(0.5, 1.6, 0.4, 0.7); /* Yaylanma eğrisi */
}
```

## 🚀 Nasıl Kullanılır?
Proje dosyalarını indirin.

index.html dosyasını favori tarayıcınızda açın.

Butonların üzerine gelin ve farklı eksenlerdeki (X ve Y) dolgu efektlerini deneyimleyin.

## 👨‍💻 Neler Öğrenildi?
::before psödo-elemanı ile HTML'i kirletmeden görsel katman ekleme.

transform-origin ile animasyon yönünü kontrol etme.

cubic-bezier ile standart dışı hız eğrileri tasarlama.

absolute konumlandırmada translate ile tam merkezleme yapma.
