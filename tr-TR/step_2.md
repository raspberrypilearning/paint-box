## Kalem yapmak

Sahne Alanı'nda çizim için kullanabileceğiniz bir kalem yaparak başlayın.

\--- task \--- Scratch başlangıç projesi; 'Boya kutusu' nu açın.

**Çevrimiçi**: başlangıç projesini [rpf.io/paint-box-on](http://rpf.io/paint-box-on){: target = "_ blank"} linkinden açın

Eğer bir Scratch hesabınız varsa, **Remix**'e tıklayarak bir kopyasını oluşturabilirsiniz.

** Çevrimdışı**: [başlangıç projesini](http://rpf.io/p/en/paint-box-go) Çevrimdışı düzenleyicide {: target = "_ blank"} açın.

Scratch çevrimdışı düzenleyicisini indirip yüklemeniz gerekirse, bunu [ rpf.io/scratchoff adresinden bulabilirsiniz. ](http://rpf.io/scratchoff) {: Hedef = "_ blank"}

Başlangıç projesinde kurşun kalem ve silgi kuklalarını görmelisiniz:

![ekran görüntüsü](images/paint-starter.png) \--- /task \---

\--- task \---

Kalem uzantısını projenize ekleyin.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Kuklanın, fare işaretçisini `sonsuza dek`{:class="block3control"} takip etmesi için kurşun kalem kuklasına biraz kod ekleyin, böylece çizebileceksiniz:

![kalem](images/pencil.png)

```blocks3
yeşil bayrak tıklandığında
sürekli tekrarla 
  (fare imleci) 'e git
end
```

\--- /task \---

\--- task \--- Bayrağa tıklayın ve ardından kodunuzun işe yarayıp yaramadığını test etmek için fare işaretçisini Sahne Alanı çevresinde hareket ettirin. \--- /task \---

Şimdi, kaleminizi `sadece fareye tıklandığında`{:class="block3control"}ekranda çizim yapacak şekilde ayarlayalım.

\--- task \--- Bu kodu kalem kuklanıza ekleyin:

![kalem](images/pencil.png)

```blocks3
yeşil bayrak tıklandığında
sürekli tekrarla 
  (fare imleci) 'e git

  eğer <mouse down?> ise 
  kalemi bastır
  değilse 
  kalemi kaldır
end
```

\--- /task \---

\--- task \--- Kodunuzu tekrar test edin. Bu kez, kalemi Sahne Alanı çevresinde hareket ettirin ve fare düğmesini basılı tutun. Kaleminle çizim yapabiliyor musun?

![ekran görüntüsü](images/paint-draw.png) \--- /task \---

## \--- collapse \---

## title: Kalemin ucundan çizmiyor mu?

Kaleminizin çizdiği çizgi kalemin ortasından geliyor gibi görünüyorsa, kalem kuklanızı değiştirmeniz gerekir, böylece ucu kuklanın merkezi olur.

Kalem kuklasına ve ardından **Kostüm** sekmesine tıklayın.

Kostümü hareket ettirin, böylece kalemin ucu merkezin **hemen yukarısında** kalacaktır.

![Kostüm merkezi](images/costume-center-annotated.png)

Şimdi kalemi Sahne Alanı'nda dolaştırın ve çizin. Artık kalem çizgiyi ucundan çizecektir.

\--- /collapse \---