## Renkli kalemler

Şimdi projenize farklı renkli kalemler ekleyeceksiniz ve kullanıcının aralarından seçim yapmasına izin vereceksiniz.

\--- task \--- ` kalemini `tükenmez kalem mavisi</code>ne değiştirin

![rename-pencil](images/rename-pencil.png) \--- /task \---

\--- task \--- Right click on the pencil sprite, and duplicate the 'pencil-blue' costume.

![ekran görüntüsü](images/paint-blue-duplicate.png) \--- /görev \---

\--- task \--- Name the new costume 'pencil-green', and colour the pencil green.

![ekran görüntüsü](images/paint-pencil-green.png)

\--- /task \---

\--- task \--- Draw two new sprites: one blue square and one green square. These are for choosing between the blue and green pencil.

![ekran görüntüsü](images/paint-selectors.png) \--- /task \---

\--- task \--- Rename the new sprites so that they are called 'blue' and 'green'

[[[generic-scratch3-rename-sprite]]]

\--- /görev \---

\--- task \--- Add some code to the 'green' sprite so that when this sprite is clicked, it `broadcasts`{:class="block3events"} the message "green".

![green square](images/green_square.png)

```blocks3
bu sprite
yayını tıkladığında (yeşil v)
```

[[[generic-scratch3-broadcast-message]]] \--- /task \---

The pencil sprite should listen for the "green" message and change its costume and pencil colour in response.

\--- task \--- Switch to your pencil sprite. Add some code so that when this sprite receives the `green`{:class="block3events"} broadcast, it switchs to the green pencil costume and changes the pen colour to green.

![kalem](images/pencil.png)

```blocks3
[yeşil v]
kostümünü aldığımda (kalem-yeşil v)
set kalem rengini [# 00CC44]
```

To set the pencil to colour to green, click the coloured square in the `set pen color`{:class="block3extensions"} block, and then click on the green square sprite. \--- /görev \---

Then to a similar thing so that you can switch the pencil colour to blue.

\--- task \--- Click on the blue square sprite and add this code:

![blue_square](images/blue_square.png)

```blocks3
bu sprite
yayını tıkladığında (mavi v)
```

Then click on the pencil sprite and add this code: ![kalem](images/pencil.png)

```blocks3
[mavi v]
kostümünü değiştirdiğimde (kalem-mavi v)
set kalem rengi [# 0000ff]
```

\--- /görev \---

\--- task \--- Finally, add this code to tell the pencil sprite which colour to start with, and to make sure that the screen is clear when your program starts.

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

\--- /görev \---

If you prefer, you can start with a different colour pencil.

\--- task \--- Test your code. Can you switch between the blue and green pencil colours by clicking on the blue or green square sprites?

![ekran görüntüsü](images/paint-pens-test.png) \--- /görev \---