## Kalem yapmak

Sahne Alanı'nda çizmek için kullanabileceğiniz bir kalem yaparak başlayın.

\--- görev \--- 'Çizim kutusu' Çizilmeye başlama projesini açın.

**Çevrimiçi**: başlangıç projesini [rpf.io/paint-box-on](http://rpf.io/paint-box-on){: target = "_ blank"}

**Çevrimdışı**: Çevrimdışı düzenleyicide [başlangıç projesi](http://rpf.io/p/en/paint-box-go){: target = "_ blank"} açın.

Scratch çevrimdışı düzenleyicisini indirip yüklemeniz gerekirse, bunu [rpf.io/scratchoff](http://rpf.io/scratchoff){: target = "_ blank"} konumunda bulabilirsiniz.

Başlangıç projesinde kurşun kalem ve silgi spritelarını görmelisiniz:

![ekran alıntısı](images/paint-starter.png) \--- /task \---

\--- task \---

Pen uzantısını projenize ekleyin.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Sprite kalemini `sonsuza kadar`fare işaretçisini takip etmesi için bazı kodlar ekleyin {: class = "block3control"}, böylece çizebilirsiniz:

![kalem](images/pencil.png)

```blocks3
bayrak
sonsuza kadar
  tıklatıldığında, (fare işaretçisi v)
son
```

\--- /görev \---

\--- görev \--- Bayrağa tıklayın ve ardından kodunuzun çalışıp çalışmadığını test etmek için fare işaretçisini Sahne Alanı çevresinde hareket ettirin. \--- /görev \---

Ardından, kalem sadece çizmek yapmak `ise`{: class = "block3control"} fare düğmesi tıklandığında ediliyor.

\--- görev \--- Bu kodu kalem kaleminize ekleyin:

![kalem](images/pencil.png)

```blocks3
Bayrak tıklandığında
sonsuza
  (fare işaretçisi v) için gitmek

+ halinde <mouse down?> daha sonra
  kalem aşağı
  başka bir
  kalemi
uç
```

\--- /task \---

\--- görev \--- Kodunuzu tekrar test edin. Bu kez, kalemi Sahne Alanı çevresinde hareket ettirin ve fare düğmesini basılı tutun. Kaleminle çizim yapabiliyor musun?

![ekran görüntüsü](images/paint-draw.png) \--- /task \---

## \--- collapse \---

## title: Kalemin ucundan çizmiyor mu?

Kaleminizin çizdiği çizgi kalemin ortasından geliyor gibi görünüyorsa, kalem sprite'larınızı değiştirmeniz gerekir, böylece ucu sprite'nın merkezi olur.

Kalem sprite tıklayın ve sonra **Kostüm** sekmesine tıklayın.

Kostüm o kadar kalem ucu Move **hemen üstünde** merkezi.

![Kukla merkezi](images/costume-center-annotated.png)

Şimdi kalemi Sahne Alanı'nda dolaştırın ve çizin. Kalem şimdi ucundan bir çizgi çekmelidir.

\--- /collapse \---