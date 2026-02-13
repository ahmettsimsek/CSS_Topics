<img width="1918" height="1007" alt="Image" src="https://github.com/user-attachments/assets/d343380d-e020-4a6f-914a-88926789cbea" />

📦 CSS Flexbox Kısa Notlar

Flexbox, elementleri yatay veya dikey olarak hizalamayı kolaylaştıran bir CSS yerleşim sistemidir.

✅ display: flex

Bir kapsayıcıya verildiğinde içindeki tüm elementleri yan yana getirir.

.container {
  display: flex;
}

✅ flex

Alanı eşit veya orantılı paylaşmak için kullanılır.

flex:1 → Tüm kutular eşit genişlikte olur.

flex:3 ve flex:1 → Alanın 3/4’ünü biri, 1/4’ünü diğeri alır.

✅ column-gap

Kutular arasındaki boşluğu ayarlar.

container {
  column-gap: 10px;
}

✅ justify-content (Yatay Hizalama)
Değer	Açıklama
space-between	İlk ve son kutu kenarlara yapışır
space-around	Kutuların etrafında eşit boşluk olur
space-evenly	Tüm boşluklar tamamen eşittir
✅ align-items (Dikey Hizalama)
Değer	Açıklama
flex-start	Üste hizalar
center	Ortalar
flex-end	Alta hizalar

⚠️ Dikey hizalamayı görmek için kapsayıcıya height vermelisin.

🎯 Özet

display:flex → Esnek yapı kurar

flex → Alan paylaşımı yapar

justify-content → Yatay hizalar

align-items → Dikey hizalar

gap → Kutular arası boşluk verir
