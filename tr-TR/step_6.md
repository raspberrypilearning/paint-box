## Kalem genişliğini değiştirin

Ardından, programınızı kullanan kişinin farklı kalem genişlikleri olan şeyler çizmesine izin vermek için kod ekleyeceksiniz.

\--- görev \--- İlk önce, `genişlik`{: class = "block3variables"} adlı yeni bir değişken ekleyin.

[[[generic-scratch3-add-variable]]] \--- / görev \---

\--- görev \--- Bu satırı **içine** sonsuza kadar `ekleyin`{: class = "block3control"} kalem sprite kodunun döngüsü:

```blocks3
Bayrak tıklandığında
silme her
(kalem mavisi v) geçiş kostüm
[# 0035FF] set kalem rengi
sonsuza
git (fare işaretçisi v) için
+ set kalem büyüklüğü (genişliği :: değişkenlere)
ise <<mouse down?> ve <(fare y) > [-120]>> sonra 
  aşağı kalem
  başka
  aşağı kalem
uç
```

\--- /görev \---

Kalem genişliği şimdi tekrar tekrar `genişlik`{: class = "block3variables"} değişkeninin değerine ayarlanır.

\--- görev \--- Sahne Alanı'nda görüntülenen `genişlik`{: class = "block3variables"} değişkenine sağ tıklayın ve ardından **kaydırıcı**tıklayın.

![ekran alıntısı](images/paint-slider.png) \--- /görev \---

Artık değişkenin değerini değiştirmek için değişkenin altında görünen kaydırıcıyı sürükleyebilirsiniz.

![ekran alıntısı](images/paint-slider-change.png)

\--- görev \--- Projenizi test edin ve kalem genişliğini ayarlamak için kod ekleyip ekleyemeyeceğinizi görün.

![ekran görüntüsü](images/paint-width-test.png) \--- /görev \---