## Pensil berwarna

Mari kita tambahkan pensil berwarna lain ke proyek kamu, dan ijinkan pengguna untuk memilih di antara mereka.

+ Klik sprite pensil kamu, klik 'Kostum' dan gandakan kostum 'pensil-biru' kamu.

![tangkapan layar](images/paint-blue-duplicate.png)

+ Ganti nama kostum baru menjadi 'pensil-hijau', dan warnai pensil hijau.

![tangkapan layar](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ Gambar dua sprite baru - satu kotak biru dan satu kotak hijau. Kamu akan menggunakan mereka untuk memilih pensil biru atau hijau.

![tangkapan layar](images/paint-selectors.png)

+ Ganti nama sprite kamu sehingga mereka disebut 'biru' dan 'hijau'

+ Tambahkan beberapa kode ke sprite 'hijau' sehingga ketika diklik, pesan "hijau" akan di-`siarkan`{:class="blockevents"} ke sprite pensil, memberitahu dia untuk mengubah kostum dan warnanya.

![Siarkan hijau](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Beralih ke sprite pensil kamu. Tambahkan beberapa kode sehingga ketika sprite ini `menerima`{:class="blockevents"} pesan "hijau", dia harus beralih ke kostum pensil hijau dan mengubah warna menjadi hijau.

![Siarkan hijau](images/broadcast-green.png)

Untuk mengatur pensil ke warna hijau, klik kotak berwarna di blok `atur warna pena`{:class="blockpen"}, dan klik pada sprite hijau untuk memilih warna hijau tersebut sebagai warna pensil kamu.

+ Kamu sekarang dapat melakukan hal yang sama untuk ikon pensil biru: tambahkan kode ini ke sprite kotak biru:

```blocks
ketika sprite ini diklik
siarkan pesan [biru v]
```

...dan tambahkan kode ini ke sprite pensil:

```blocks
ketika aku menerima [biru v]
ganti kostum ke [pensil-biru v]
atur warna pena ke [#0000ff]
```

+ Terakhir, tambahkan kode ini untuk memberi tahu sprite pensil yang mana warna awalnya, dan pastikan bahwa layarnya bersih.

![Mulai pensil](images/start-pencil.png)

Kami memilih untuk memulai dengan warna biru tapi jika kamu suka, kamu dapat memulai dengan pensil warna lain.

+ Uji proyek Anda. Dapatkah Anda beralih antara pena biru dan hijau dengan mengklik sprite kotak biru atau hijau?

![tangkapan layar](images/paint-pens-test.png)