## Renkli kalemler

Şimdi projenize farklı renkli kalemler ekleyeceksiniz ve kullanıcının aralarından seçim yapmasına izin vereceksiniz.

\--- görev \--- Kalem kalemine tıklayın, **Kostüm**tıklayın ve 'kalem mavisi' kostümünü çoğaltın.

![ekran görüntüsü](images/paint-blue-duplicate.png) \--- /task \---

\--- görev \--- Yeni kostümü 'kurşun yeşili' olarak adlandırın ve kurşun kalem yeşilini renklendirin.

![ekran görüntüsü](images/paint-pencil-green.png)

\--- /task \---

\--- görev \--- İki yeni sprite çiz: bir mavi kare ve bir yeşil kare. Bunlar mavi ve yeşil kalem arasında seçim yapmak için.

![ekran alıntısı](images/paint-selectors.png) \--- /task \---

\--- görev \--- Yeni karakterleri 'mavi' ve 'yeşil' olarak adlandırılacak şekilde yeniden adlandırın.

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- görev \--- 'yeşil' sprite bazı kodu ekleyin, böylece bu sprite tıklandığında, o `yayın`{: class = "block3events"} mesaj "yeşil".

![yeşil kare](images/green_square.png)

```blocks3
bu sprite
yayını tıkladığında (yeşil v)
```

[[[generic-scratch3-broadcast-message]]] \--- / görev \---

Kalem sprite "yeşil" mesajı dinlemeli ve karşılık olarak kostümünü ve kalem rengini değiştirmelidir.

\--- görev \--- Kalem kaleminize geçin. Bu sprite `yeşil`{: class = "block3events"} yayınını aldığında, yeşil kalem kostüme geçiş yapmak ve kalem rengini yeşile dönüştürmek için bazı kodlar ekleyin.

![kalem](images/pencil.png)

```blocks3
[yeşil v]
kostümünü aldığımda (kalem-yeşil v)
set kalem rengini [# 00CC44]
```

Kalemi yeşile ayarlamak için, `set kalem rengi`{: class = "block3extensions"} bloğundaki renkli kareye tıklayın ve ardından yeşil kare sprite tıklayın. \--- /task \---

Sonra da benzer bir şeye, böylece kurşun kalem rengini maviye çevirebilirsin.

\--- görev \--- Mavi kareye tıklayın ve şu kodu ekleyin:

![blue_square](images/blue_square.png)

```blocks3
bu sprite
yayını tıkladığında (mavi v)
```

Ardından kalem sprite üzerine tıklayın ve şu kodu ekleyin: ![kalem](images/pencil.png)

```blocks3
[mavi v]
kostümünü değiştirdiğimde (kalem-mavi v)
set kalem rengi [# 0000ff]
```

\--- /görev \---

\--- görev \--- Son olarak, kalem sprite'e hangi rengin başlayacağını söylemek ve program başladığında ekranın açık olduğundan emin olmak için bu kodu ekleyin.

![kalem](images/pencil.png)

```blocks3
Bayrak tıklandığında
+ bütün silmek
+ (kalem-mavi V) kostüm geçiş
+ set kalem rengi [# 0035FF] için
sonsuza
  git (fare işaretçisi v) için
ise <mouse down?> daha sonra
  kalem aşağı
  başka
  kalemi
son
```

\--- /task \---

İsterseniz farklı bir renkli kalemle başlayabilirsiniz.

\--- görev \--- Kodunuzu test edin. Mavi ya da yeşil kalem renkleri arasında geçiş yaparak mavi ve yeşil kalem renkleri arasında geçiş yapabilir misiniz?

![ekran görüntüsü](images/paint-pens-test.png) \--- /task \---