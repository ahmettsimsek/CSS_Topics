<img width="1912" height="1047" alt="Image" src="https://github.com/user-attachments/assets/7c900f8b-e3fc-4ba6-b370-65650758754d" />

<img width="1905" height="668" alt="Image" src="https://github.com/user-attachments/assets/ad6df887-d0a4-4cef-b657-1a7cb898a506" />

<img width="1894" height="885" alt="Image" src="https://github.com/user-attachments/assets/bd1eea7f-fc85-4813-ac9c-4b532b2046ea" />

<img width="1908" height="870" alt="Image" src="https://github.com/user-attachments/assets/48fd5e78-5e25-4f08-947c-59e26e3f8a3f" />

📐 CSS Grid Temelleri

Bu proje, CSS Grid yapısının temel özelliklerini öğrenmek ve görsel olarak test etmek amacıyla hazırlanmıştır.
Farklı grid özellikleri örnek kutular üzerinden gösterilmiştir.

🚀 Kullanılan Konular
1️⃣ display: grid

Bir kapsayıcıya display: grid; verildiğinde içindeki elemanlar grid sistemi ile hizalanır.

'''css

display: grid;

'''

2️⃣ grid-template-columns

Bir satırda kaç kolon olacağını ve genişliklerini belirler.

grid-template-columns: 100px 100px;


Örnek:

2 kolon → 100px + 100px

4 kolon → 100px 100px 100px 500px

3️⃣ fr Birimi (Flexible Unit)

fr birimi, kalan boş alanı eşit şekilde dağıtır.

grid-template-columns: 1fr 1fr 1fr;


Bu kullanım:

3 eşit kolon oluşturur

Sayfa genişliğine göre otomatik uyum sağlar

4️⃣ column-gap

Kolonlar arası yatay boşluk bırakır.

column-gap: 10px;

5️⃣ row-gap

Satırlar arası dikey boşluk bırakır.

row-gap: 10px;

6️⃣ gap

Hem yatay hem dikey boşluğu tek satırda verir.

gap: 20px;


Bu kullanım:

row-gap + column-gap yerine geçer.

📌 Projede Gösterilen Senaryolar

✔ Sabit genişlikli grid
✔ Karışık kolon yapısı
✔ fr ile esnek grid
✔ Eşit kolon sistemi
✔ Kolon arası boşluk
✔ Satır arası boşluk
✔ Genel boşluk kullanımı

🎯 Amaç

Bu proje sayesinde:

CSS Grid mantığını kavrama

fr birimini anlama

Grid boşluk sistemini öğrenme

Responsive yapının temelini görme
