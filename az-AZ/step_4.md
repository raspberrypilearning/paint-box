## Rəngli qələmlər

Layihəinizə müxtəlif rəngli qələmlər əlavə edək və istifadəçi arasında seçim etməyə icazə verək.

+ Qələm sprite vurun, 'Costumes' düyməsini basın və 'qələm-mavi' kostyumunu çoğaltın.

![ekran görüntüsü](images/paint-blue-duplicate.png)

+ Yeni kostyumunuzu 'qələm-yaşıl' adını dəyişin və qələm yaşıl rəngini rəngləndirin.

![ekran görüntüsü](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ Iki yeni sprites - bir mavi kvadrat və bir yaşıl kvadrat çəkin. Mavi və ya yaşıl qələm seçmək üçün bunları istifadə edəcəksiniz.

![ekran görüntüsü](images/paint-selectors.png)

+ Spritlerinizi "mavi" və "yaşıl" adlandırmaq üçün yenidən adlandırın

+ "Yaşıl" spritə bir neçə kod əlavə etsin ki, tıklandığında `kostyum və qələm rəngini dəyişdirməyi izah edən qələm spritə "yaşıl" mesajını`{: class = "blockevents"} yayır.

![Yaşıl yayılmaq](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Qələm spritinə keçin. Bu sprite `yayımını`{: class = "blockevents"} yaşıl qəbul edərkən, o, yaşıl qələm kostyuma keçir və qələm rəngini yaşıl dəyişdirmək üçün bir sıra kod əlavə edin.

![Yaşıl yayılmaq](images/broadcast-green.png)

Qələmi rəngə düzəldmək üçün `set qələm rənginin`{: class = "blockpen"} blokunun rəngli qutusuna basın və qələm rənginizlə eyni rəngli yaşıllığı seçmək üçün yeşil sprite vurun.

+ İndi mavi qələm simvolu üçün eyni şeyi edə bilərsiniz: bu kodu mavi kvadrat sprite əlavə edin:

```blocks
bu sprite yayımda [mavi v]
```

... və bu kodu qələm sprite əlavə edin:

```blocks
[blue v] keçid kostyumunu [pencil-mavi v] qələm rəngini [# 0000ff]
```

+ Nəhayət, bu kodu qələmi sprite ilə başlayan rəngi izah etmək üçün əlavə edin və ekranın təmiz olduğundan əmin olun.

![Qələm başlayın](images/start-pencil.png)

Mavi ilə başlamağı seçdik, ancaq tercih etsəniz fərqli bir rəng qələmlə başlaya bilərsiniz.

+ Layihənizi test edin. Mavi və ya yaşıl kvadrat sprites tıklayarak mavi və yaşıl qələm arasında keçid edə bilərəmmi?

![ekran görüntüsü](images/paint-pens-test.png)