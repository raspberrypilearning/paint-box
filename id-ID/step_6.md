## Mengubah lebar pensil

Mari kita ijinkan pengguna untuk menggambar dengan beragam ukuran pensil yang berbeda.

+ Pertama, tambahkan variabel baru bernama `lebar`{:class="blockvariable"}.

[[[generic-scratch-add-variable]]]

+ Tambahkan baris ini *di dalam* pengulangan `selamanya`{:class="blockcontrol"} pada kode pensil:

```blocks
    atur ukuran pena ke (lebar)
```

Lebar pensil sekarang akan berulang kali diatur ke nilai variabel 'lebar'.

+ Klik kanan pada tampilan variabel di stage dan klik 'slider'.

![tangkapan layar](images/paint-slider.png)

Kamu sekarang dapat menyeret slider di bawah variabel untuk mengubah nilainya.

![tangkapan layar](images/paint-slider-change.png)

+ Uji proyek kamu, dan lihat jika kamu dapat mengubah lebar pensil.

![tangkapan layar](images/paint-width-test.png)

Jika kamu suka, kamu dapat mengatur nilai terkecil dan terbesar dari 'lebar' yang diijinkan. Untuk melakukan ini, klik kanan lagi pada tampilan variabel dan klik 'set min dan max slider'. Atur nilai terkecil dan terbesar dari variabel kamu ke sesuatu yang lebih masuk akal, seperti 1 dan 20.

![tangkapan layar](images/paint-slider-max.png)

Terus uji variabel 'lebar' sampai kamu puas.