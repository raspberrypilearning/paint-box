## Renkli kalemler

Projenize farklı renkli kalemler ekleyelim ve kullanıcının aralarında seçim yapmasına izin verelim.

+ Kalem kukla'nıza tıklayın, 'Kılık'ı tıklayın ve 'kalem-mavi' kostümünüzü kopyalayın.

![ekran görüntüsü](images/paint-blue-duplicate.png)

+ Yeni kılığınızı 'kalem-yeşil' olarak adlandırın ve yeşil kalemle renklendirin.

![ekran görüntüsü](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ İki yeni kukla çizin - bir mavi kare ve bir yeşil kare. Mavi veya yeşil kalem seçmek için bunları kullanacaksınız.

![ekran görüntüsü](images/paint-selectors.png)

+ Kuklalarınızın isimlerini değiştirin. Bu sayede 'mavi' ve 'yeşil' olarak seçebiliriz.

+ 'yeşil' kuklasına bazı kodlar ekleyelim. Böylece tıklandığında, kalem kuklasının kılığını ve kalem rengini değiştirmesi anlamına gelen "yeşil" mesajını `yayınlasın`{:class="blockevents"}.

![Yeşil yayın](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Kalem kuklanıza geçin. Bazı kodlar ekleyelim. Böylece `yayınlanan`{:class="blockevents"} yeşil mesajını alan kukla, yeşil kalem kılığına geçsin ve kalemin rengini yeşil yapsın.

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