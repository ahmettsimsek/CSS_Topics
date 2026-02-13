# CSS Display Özelliği

CSS'te **display** özelliği, bir HTML elementinin sayfada nasıl görüneceğini ve diğer elementlerle nasıl hizalanacağını belirler.

Temel olarak iki ana görünürlük türü vardır:

* **Block (Blok)**
* **Inline (Satır içi)**

Ayrıca bu ikisinin birleşimi olan **inline-block** da sıkça kullanılır.

---

## 🔹 Block Elementler

Block elementler bulundukları satırın **tamamını kaplar** ve her zaman yeni bir satırdan başlar.

### Özellikleri:

✅ Tüm satırı kaplar
✅ Genişlik (`width`) ve yükseklik (`height`) verilebilir
✅ Margin ve padding değerleri tam olarak uygulanır

### Örnek Block Etiketleri:

```html
<div></div>
<p></p>
<h1></h1>
<section></section>
```

### CSS Örneği:

```css
div {
  display: block;
  width: 300px;
  height: 100px;
}
```

---

## 🔹 Inline Elementler

Inline elementler sadece **içerikleri kadar yer kaplar** ve yeni satıra geçmezler.

### Özellikleri:

✅ Yan yana dizilirler
❌ `width` ve `height` genellikle uygulanmaz
❌ Üst ve alt margin sınırlı çalışır

### Örnek Inline Etiketleri:

```html
<span></span>
<a></a>
<strong></strong>
```

### CSS Örneği:

```css
span {
  display: inline;
}
```

---

## 🔹 Inline-Block

`inline-block`, hem inline hem de block özelliklerini birleştirir.

👉 Elementler **yan yana durur** ama aynı zamanda **width ve height** verilebilir.

### Ne Zaman Kullanılır?

* Kart tasarımları
* Menü öğeleri
* Butonlar
* Galeri yapıları

### CSS Örneği:

```css
.card {
  display: inline-block;
  width: 200px;
  height: 150px;
}
```

---

## 🔹 Display ile Tür Değiştirme

CSS sayesinde bir elementin varsayılan davranışını değiştirebilirsiniz.

### Inline ➜ Block

```css
span {
  display: block;
}
```

### Block ➜ Inline

```css
div {
  display: inline;
}
```

### Block ➜ Inline-Block

```css
div {
  display: inline-block;
}
```

---

## 🎯 Özet Tablo

| Özellik                    | Inline | Block | Inline-Block |
| -------------------------- | ------ | ----- | ------------ |
| Satırın tamamını kaplar    | ❌      | ✅     | ❌            |
| Yan yana durur             | ✅      | ❌     | ✅            |
| Width / Height verilebilir | ❌      | ✅     | ✅            |
| Yeni satırdan başlar       | ❌      | ✅     | ❌            |

---

## ✅ Kısaca:

* **Inline:** İçeriği kadar yer kaplar.
* **Block:** Tüm satırı kaplar.
* **Inline-block:** Yan yana durur ama boyutlandırılabilir.

---

İyi bir CSS yerleşimi (layout) kurabilmek için `display` özelliğini anlamak çok önemlidir 🚀
