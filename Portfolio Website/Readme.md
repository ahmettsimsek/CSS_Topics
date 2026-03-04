<img width="1908" height="974" alt="Image" src="https://github.com/user-attachments/assets/f65d0180-ef6f-417a-9830-92698e457c84" />

# 🌐 Modern Portfolio Website

Bu proje, HTML5 ve CSS3 kullanılarak geliştirilmiş, animasyonlarla zenginleştirilmiş modern bir kişisel portfolyo web sitesidir. Kullanıcı deneyimini ön plana çıkaran akıcı geçişler ve tamamen duyarlı (responsive) bir tasarım sunar.

## ✨ Öne Çıkan Özellikler

- **Dinamik Yazı Efekti (Typing Animation):** `@keyframes` ve `::before/::after` psödo-elemanları kullanılarak yapılan, JavaScript gerektirmeyen otomatik yazı değiştirme özelliği.
- **Modern UI/UX Tasarımı:** Poppins yazı tipi, karanlık mod teması ve `#b74b4b` vurgu rengi ile estetik bir görünüm.
- **Tam Duyarlı Tasarım (Responsive):** Media Queries kullanılarak mobil, tablet ve masaüstü cihazlar için optimize edilmiş yapı.
- **Gelişmiş Hover Efektleri:** Sosyal medya ikonlarında ve logoda `transform`, `scale` ve `box-shadow` kombinasyonları ile etkileşimli geri bildirimler.
- **Fixed Navigation:** Sayfa kaydırılsa bile üstte sabit kalan, `drop-shadow` filtreli modern menü.

---

## 🛠️ Kullanılan Teknolojiler

- **HTML5:** Yapısal iskelet ve semantik etiketleme.
- **CSS3:** - Flexbox (Hizalama ve düzenleme)
  - Keyframes (Animasyonlar)
  - Pseudo-elements (Sanal elemanlar ile efekt yönetimi)
  - CSS Variables (Renk ve font yönetimi)
- **Font Awesome:** Sosyal medya ve arayüz ikonları.
- **Google Fonts:** Poppins font ailesi.

---

## 📦 Proje Mimarisi ve Teknik Detaylar

### 1. CSS Sıfırlama ve Kutu Modeli
Projenin temelinde tarayıcı farklılıklarını gidermek için kapsamlı bir "CSS Reset" uygulanmıştır. `box-sizing: border-box;` kullanımı ile padding ve border değerlerinin genişliği bozması engellenmiştir.

### 2. Animasyon Mantığı
Metin animasyonu, CSS `content` özelliği üzerinden yürütülmektedir. Bu sayede HTML kodu temiz tutulmuş ve tüm görsel mantık CSS tarafında toplanmıştır.

```css
@keyframes words {
    0%, 20%   { content: "Web Developer"; }
    21%, 40%  { content: "Developer"; }
    /* ... */
}
