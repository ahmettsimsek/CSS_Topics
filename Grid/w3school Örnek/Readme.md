<img width="1914" height="951" alt="Image" src="https://github.com/user-attachments/assets/dc9e3cd1-fc09-42b0-8f96-747076b4a975" />

🧩 CSS Grid Layout – Template Areas Kullanımı

Bu proje, CSS Grid Layout kullanarak klasik bir web sayfası yapısının (Header – Menu – Content – Footer) nasıl oluşturulduğunu göstermektedir.

Projede özellikle grid-template-areas özelliği kullanılmıştır.

📐 Kullanılan Grid Yapısı
🎯 grid-template-areas

Sayfa düzeni şu şekilde tanımlanmıştır:

.container {
  display: grid;
  grid-template-areas:
    "header header"
    "menu content"
    "footer footer";
}


Bu yapı:

Header → Üstte tam genişlik

Menu → Sol tarafta

Content → Sağ tarafta

Footer → Altta tam genişlik

oluşturur.

📊 Kolon Oranı
grid-template-columns: 1fr 3fr;


Bu kullanım:

Sol kolon (menu) → 1 birim

Sağ kolon (content) → 3 birim

Yani içerik alanı menüden 3 kat geniştir.

🧱 Alan Atamaları (grid-area)

Her bölüm ilgili grid alanına bağlanmıştır:

.container div.header {
  grid-area: header;
}

.container div.menu {
  grid-area: menu;
}

.container div.content {
  grid-area: content;
}

.container div.footer {
  grid-area: footer;
}

🧩 Boşluk ve Stil Ayarları
.container {
  gap: 5px;
  background-color: blue;
  padding: 5px;
}

.container div {
  background-color: aliceblue;
  padding: 10px;
}


gap → Grid elemanları arasındaki boşluk

padding → İç boşluk

Arka plan renkleri → Görsel ayrım için

📌 Oluşturulan Layout Yapısı
---------------------------------
|           HEADER              |
---------------------------------
|   MENU   |      CONTENT       |
---------------------------------
|           FOOTER              |
---------------------------------

🎯 Bu Projede Öğrenilenler

✔ grid-template-areas kullanımı
✔ grid-area ile alan eşleştirme
✔ Kolon oranı ayarlama (1fr 3fr)
✔ Basit web layout oluşturma
✔ Grid ile klasik site tasarımı
