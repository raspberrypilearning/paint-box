## Renkli kalemler

Projenize farklı renkli kalemler ekleyelim ve kullanıcının aralarında seçim yapmasına izin verelim.

+ Kalem hareketli grafiğinizi tıklayın, 'Kostümler'i tıklayın ve' kalem-mavisi 'kostümünüzü kopyalayın.

![ekran görüntüsü](images/paint-blue-duplicate.png)

+ Yeni kostümünüzü 'kurşun kalem-yeşil' olarak adlandırın ve yeşil kalemle renklendirin.

![ekran görüntüsü](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ İki yeni sprite çizin - bir mavi kare ve bir yeşil kare. Mavi veya yeşil kalem seçmek için bunları kullanacaksınız.

![ekran görüntüsü](images/paint-selectors.png)

+ Sprite'larınızı 'mavi' ve 'yeşil' olarak adlandırılacak şekilde yeniden adlandırın.

+ 'Yeşil' sprite bazı kodu ekleyin böylece tıklandığında, bu olacak `yayını`{: class = "blockevents"} bunu söylüyorum kalem sprite mesaj "yeşil", onun kılık ve kalem rengini değiştirmek için.

![Yeşil yayın](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Kurşun kaleminize geçin. Bu kod yazımı `yayın`{: class = "blockevents"} yeşili aldığında, yeşil kalem kılığına geçmeli ve kalem rengini yeşile çevirmelidir.

![Yeşil yayın](images/broadcast-green.png)

Kalemi yeşil renge ayarlamak için, `ayarlanan kalem rengi`{: class = "blockpen"} bloğundaki renkli kutuyu tıklatın ve yeşil renkte kalem renginizle aynı rengi seçmek için yeşil hareketli grafiğe tıklayın.

+ Şimdi mavi kalem simgesi için de aynısını yapabilirsiniz: bu kodu mavi kare hareketli grafiğe ekleyin:

```blocks
bu hareketli grafik yayınlandığında [mavi v]
```

... ve bu kodu kalem hareketli grafiğe ekleyin:

```blocks
[mavi v] aldığımda [kalem mavisi v] 'e kostüm değiştirdim kalem rengini [# 0000ff] olarak ayarla
```

+ Son olarak, hangi renkten başlayacağınız kalem işleyicisine anlatmak için bu kodu ekleyin ve ekranın temiz olduğundan emin olun.

![Kalem başlat](images/start-pencil.png)

Mavi ile başlamayı seçtik ama tercih ederseniz, farklı bir renk kalemle başlayabilirsiniz.

+ Projenizi test edin. Mavi veya yeşil kare spriteları tıklayarak mavi ve yeşil kalemler arasında geçiş yapabilir misiniz?

![ekran görüntüsü](images/paint-pens-test.png)