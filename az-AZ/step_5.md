## Səhv etmək

Bəzən səhvlər olur, buna görə də 'təmiz' düyməsini və silgi əlavə edək.

+ 'X-block' sprite əlavə edin - onu kitabxanada məktublar bölümündə tapa bilərsiniz. Kıyafeti qırmızı rəngdə rəngləndirin. Bu, 'aydın' düyməsinə çevriləcəkdir.

![ekran görüntüsü](images/paint-x.png)

+ Çağırıldıqda səhnəni təmizləmək üçün bu sprite kodu əlavə edin.

![Səhnəni təmizləyin](images/clear-stage.png)

Səhnəni təmizləmək üçün bir mesaj göndərməyinizə ehtiyac olmadığını nəzərə alsaq, bu sprite olan açıq bloku istifadə edə bilərsiniz.

Yəqin ki, qələm spritinizin silgi kostyumunu ehtiva etdiyini fərq etmişsiniz:

![ekran görüntüsü](images/paint-eraser-costume.png)

+ Projeniz ayrıca ayrı silgi sprite də daxildir. Bu sprite sağ basın və 'show' seçin. Səhnə necə baxmaq lazımdır:

![ekran görüntüsü](images/paint-eraser-stage.png)

+ Spreyin vurulduğu zaman qələmi bir silgiyə keçirməyi izah etmək üçün silgi spritinə kod əlavə edin.

![Broadcast silgi](images/broadcast-eraser.png)

Qələm "pozan" mesajı aldığında, qələm kostyumunu pozanya dəyişə bilərsiniz və qələm rəngini ağa dəyişə bilərsiniz - səhnə ilə eyni rəng!

+ Silgi yaratmaq üçün bir neçə kod əlavə edin

\--- ipuçları \--- \--- ipucu \--- qələm sprite bir kod əlavə et: **** aldığımda **silici** mesajı **kostyuma keçmək** silgi **qələm rəngini qoyun** ağa \--- / ipucu \--- \--- ipucu \--- Qələm sprite içərisində kod necə olmalıdır:

```blocks
[eraser v] keçid kostyumunu [silici v] [#FFFFFF] qələm rəngini [
```

\--- / ipucu \--- \--- / göstərişlər \---

+ Səhnədə silmək və silinməyiniz üçün layihəni test edin.

![ekran görüntüsü](images/paint-erase-test.png)

Qələm ilə bir problem daha var - səhnədə hər hansı bir yerə çəkə bilərsiniz, o cümlədən seçici nişanlarının yanında!

![ekran görüntüsü](images/paint-draw-problem.png)

Bunu düzəltmək üçün, siçanı y-mövqeyi -120-dən çox olduqda, *və* siçan tıklandığında cəlb etmək üçün qələmə bildirin:

![ekran görüntüsü](images/pencil-gt-code.png)

+ Layihənizi test edin; indi seçmə bloklarına yaxınlaşa bilməyəcəksiniz.

![ekran görüntüsü](images/paint-fixed.png)