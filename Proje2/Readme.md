<img width="1901" height="966" alt="Image" src="https://github.com/user-attachments/assets/31c779b0-eeab-4b8d-aa9c-5f02e00ab360" />

<img width="1896" height="974" alt="Image" src="https://github.com/user-attachments/assets/add440e9-2cdb-48a9-b149-835f06a51c5e" />

<img width="1893" height="975" alt="Image" src="https://github.com/user-attachments/assets/91914d89-c278-4ed2-9d7f-9ed33c27b687" />

<img width="1902" height="967" alt="Image" src="https://github.com/user-attachments/assets/769215c1-5600-4ac1-aa9e-83c1387486d9" />

<img width="1897" height="960" alt="Image" src="https://github.com/user-attachments/assets/12bb35be-065c-4199-a52f-02e7b690a08d" />

<img width="1902" height="552" alt="Image" src="https://github.com/user-attachments/assets/e9d53cb6-0210-4524-88c1-82b91e32941a" />

'''

#🌿 Nature Landing Page

Responsive (mobil uyumlu) bir Landing Page projesidir.
HTML, CSS ve temel JavaScript kullanılarak geliştirilmiştir.

# 🚀 Proje Hakkında

Bu proje:

Modern bir landing page tasarımını içerir

Mobil uyumlu responsive yapıdadır

CSS Flexbox kullanılmıştır

Mobil menü için JavaScript ile toggle sistemi eklenmiştir

Hover animasyonları ve geçiş efektleri bulunmaktadır

# 🛠️ Kullanılan Teknolojiler

HTML5

CSS3

Flexbox

Media Query

JavaScript (DOM Manipulation)

Google Fonts (DM Sans & Forum)

# 📱 Responsive Özellik

520px altındaki ekranlarda:

Menü ikon haline dönüşür

Navigation sağdan kayan mobil menü olur

Section yapıları dikey hizalanır

Footer kolon yapısı alt alta geçer

Mobil menü çalışma mantığı:
```
const navBtn = document.querySelector(".menu-btn")
const navList = document.querySelector(".nav-list")

navBtn.addEventListener("click", function() {
    navList.classList.toggle("active");
});
```

CSS tarafı:

``` css
.nav-list {
    position: absolute;
    right: -900px;
    transition: all 0.3s ease;
}

.nav-list.active {
    right: 0;
}

```

# 🎨 Proje Bölümleri

Hero Section

Services Section

Testimonial Section

About Us Section

Questions CTA Section

Footer

# ✨ Özellikler

Smooth hover zoom efekti (services ve about image)

CSS değişkenleri (:root)

Tam ekran hero arka plan

Buton tasarım sistemi (btn-primary, btn-secondary)

Flexbox layout sistemi
```

# 📂 Klasör Yapısı
project/
│
├── index.html
├── style.css
└── img/
    ├── logo.png
    ├── menu.png
    ├── main-2.jpg
    ├── service-1.jpg
    ├── service-2.jpg
    ├── service-3.jpg
    ├── about.jpg
    └── ...
```
# 🎯 Öğrenilen Konular

Bu projede:

position: absolute kullanımı

Responsive navbar yapımı

Flexbox düzeni

CSS hover animasyonları

Media Query mantığı

JavaScript ile class toggle işlemi

pratik edilmiştir.

# 📌 Geliştirilebilir Alanlar

Menüye animasyonlu ikon dönüşümü (hamburger → X)

Scroll animasyonları eklenebilir

Form validation sistemi eklenebilir

Dark mode desteği eklenebilir

# 👨‍💻 Geliştirici

Ahmet Şimşek
Computer Engineer

'''
