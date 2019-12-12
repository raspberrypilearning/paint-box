## Kalem genişliğini değiştirin

Sırada, programınızı kullanan kişinin nesneleri farklı kalem genişlikleriyle çizmesine izin veren kodu ekleyeceksiniz.

\--- görev \--- İlk önce, `genişlik`{: class="block3variables"} adlı yeni bir değişken ekleyin.

[[[generic-scratch3-add-variable]]] \--- /task \---

\--- task \--- Bu satırı kalem kuklası kodundaki `sonsuza kadar`{:class="block3control"} döngüsünün **içine** ekleyin:

```blocks3
yeşil bayrak tıklandığında
tümünü sil
(mavi-kalem) kılığına geç
kalem rengini [#0035FF] yap
sürekli tekrarla 
  (fare imleci) 'e git
  kalem kalınlığını (genişlik) yap
  eğer <<mouse down?> ve <(fare y) > [-120]>> ise 
    kalemi bastır
  değilse 
    kalemi kaldır
 end
```

\--- /task \---

Kalem genişliği şimdi hep `genişlik`{:class="block3variables"} değişkeninin değerine ayarlanır.

\--- görev \--- Sahne Alanı'nda görüntülenen `genişlik`{:class="block3variables"} değişkenine sağ tıklayın ve ardından **slider**'ı tıklayın.

![ekran alıntısı](images/paint-slider.png) \--- /task \---

Artık değişkenin değerini ayarlamak için değişkenin altında görünen kaydırıcıyı sürükleyebilirsiniz.

![ekran alıntısı](images/paint-slider-change.png)

\--- task \--- Projenizi test edin ve kalem genişliğini ayarlamak için kod ekleyip ekleyemeyeceğinizi görün.

![ekran alıntısı](images/paint-width-test.png) \--- /task \---