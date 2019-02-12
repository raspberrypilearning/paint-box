## Hataları geri al

Bazen hatalar olur, bu yüzden bir 'temizle' butonu ve bir silgi butonu ekleyin.

\--- görev \--- Kütüphanenin harfler bölümünden 'X-blok' sprite ekleyin. Sprite kostümünü kırmızıyla renklendirin ve biraz daha küçük hale getirin. Bu sprite 'temizle' düğmesidir.

[[[generic-scratch3-sprite-from-library]]]

![ekran görüntüsü](images/paint-x.png) \--- /task \---

\--- görev \--- Sprite tıkladığında Sahne Alanı'nı temizlemek için 'X-blok' sprite kodunu ekleyin.

![çapraz](images/cross.png)

```blocks3
bu sprite
tıklandığında tümünü sil
```

\--- /görev \---

Sahne Alanı'nı temizlemek için `yayın`kullanmanıza gerek yoktur; çünkü `,`{: class = "block3extensions"} bloğunun hepsini sildiğinde bu işlem yapılır.

Kalem sprite bir silgi kostümü içerdiğini görüyor musunuz?

![ekran görüntüsü](images/paint-eraser-costume.png)

Projeniz ayrıca ayrı bir silgi sprite içerir.

\--- görev \--- Bu silgi sprite öğesine sağ tıklayın ve ardından **show**tıklayın. Aşamalarınızın şimdi nasıl görünmesi gerektiği:

![ekran görüntüsü](images/paint-eraser-stage.png) \--- /task \---

\--- görev \--- Silgi sprite tıklandığında `'silgi' yayın`{: class = "block3events"} göndermek için silgi sprite kodunu ekleyin.

![silgi](images/eraser.png)

```blocks3
bu sprite
yayını tıkladığında (silgi v)
```

\--- /görev \---

Kalem sprite 'silgi' mesajını aldığında, kostümünü silgiye dönüştürmeli ve kalem rengini beyaza değiştirmelidir, bu da Sahne Alanı ile aynı renktir!

\--- görev \--- Silgiyi oluşturmak için bir kod ekleyin.

\--- ipuçları \--- \--- ipucu \--- Kalem sprite'ına bazı kodlar ekleyin: ``{: class = "block3events"} aldığımda `silgisi`{: class = "block3events"} mesaj `Kostüm silgisine geç`{: class = "block3looks"} `Kalem rengini ayarla`{: class = "block3extensions"} 'ye beyaz \--- / ipucu \--- \--- ipucu \--- İşte ihtiyacınız olan tüm bloklar:

```blocks3
[silgi v]

anahtar kostümünü (silgi v) aldığımda kalem rengini [#FFFFFF]
ayarlayın
```

\--- / ipucu \--- \--- ipucu \--- İşte kod gibi görünmelidir ne: ![kalem](images/pencil.png)

```blocks3
[silgi v]
aldığımda kostümü (silgi v)
set kalem rengini [#FFFFFF] olarak değiştir
```

\--- / ipucu \--- \--- / ipuçları \--- \--- / görev \---

\--- görev \--- Sahne Alanı'nı temizleyip kalem çizgilerini silip silemediğinizi görmek için projenizi test edin.

![ekran görüntüsü](images/paint-erase-test.png) \--- /görev \---

Kurşun kalemle ilgili bir sorun daha var: 'net' ve silgi düğmelerinin yanı sıra Sahne Alanı'nda herhangi bir yeri çizebilirsiniz!

![ekran görüntüsü](images/paint-draw-problem.png)

\--- görev \--- Bunu düzeltmek için kodu değiştirin, böylece fare yalnızca **ve** tıklatıldığında, fare işaretçisinin `y` konumu `-120`büyükse, aşağı:

![kalem](images/pencil.png)

```blocks3
bayrak tıklandığında
tüm
anahtar kostümünü sil (kalem mavisi v)
kalem rengini [# 0035FF]
sonsuza
  götür (fare imleci v)
+ eğer <<mouse down?> ve <(fare y) > [-120]>> sonra 
  aşağı kalem
  başka
  kalem yukarı
uç
```

\--- /task \---

\--- görev \--- Projenizi test edin. Şimdi düğmelerin yanına çizim yapmamalısınız.

![ekran alıntısı](images/paint-fixed.png) \--- /task \---