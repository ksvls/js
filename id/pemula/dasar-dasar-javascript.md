---
permalink: /id/pemula/dasar-dasar-javascript.html
---

# Dasar-dasar JavaScript

## Apa Itu JavaScript?

JavaScript adalah bahasa pemrograman yang menambahkan interaktivitas ke situs web Anda. Ini terjadi dalam permainan, dalam perilaku tanggapan ketika tombol ditekan atau dengan entri data pada formulir; dengan gaya dinamis; dengan animasi, dll. Artikel ini membantu Anda memulai dengan JavaScript dan memperluas pemahaman Anda tentang apa yang mungkin.

JavaScript ("JS" singkatnya) adalah bahasa pemrograman dinamis lengkap yang dapat menambahkan interaktivitas ke situs web. Itu ditemukan oleh Brendan Eich (salah satu pendiri Mozilla project, Mozilla Foundation, dan Mozilla Corporation).

JavaScript itu serbaguna dan ramah pemula. Dengan lebih banyak pengalaman, Anda akan dapat membuat game, animasi 2D dan grafik 3D, aplikasi berbasis database yang komprehensif, dan banyak lagi!


JavaScript sendiri relatif ringkas, namun sangat fleksibel. Developer lain telah menulis berbagai alat di atas bahasa JavaScript inti, membuka banyak fungsi dengan sedikit usaha. Ini termasuk:

- Browser Application Programming Interfaces (API) yang terpasang di peramban web, menyediakan fungsionalitas seperti membuat HTML secara dinamis dan menyetel gaya CSS; mengumpulkan dan memanipulasi aliran video dari webcam pengguna, atau membuat grafik 3D dan sampel audio.
- Third-party API yang memungkinkan pengembang untuk menggabungkan fungsionalitas di situs dari penyedia konten lain, seperti Twitter atau Facebook.
- Third-party frameworks dan libraries yang dapat Anda terapkan ke HTML untuk mempercepat pekerjaan membangun situs dan aplikasi.


Bagian di bawah ini memperkenalkan beberapa aspek dari bahasa inti dan menawarkan kesempatan untuk bermain dengan beberapa fitur API browser juga. Selamat mencoba!

## Sebuah contoh Hello World!

JavaScript adalah salah satu teknologi web modern paling populer! Saat keterampilan JavaScript Anda berkembang, situs web Anda akan memasuki dimensi baru kekuatan dan kreativitas.

Namun, menjadi terbiasa dengan JavaScript lebih menantang daripada merasa nyaman dengan HTML dan CSS. Anda mungkin harus memulai dari yang kecil, dan berkembang secara bertahap. Untuk memulai, mari kita periksa cara menambahkan JavaScript ke halaman Anda untuk membuat Hello world! contoh. ([Hello World! Adalah standar untuk contoh pemrograman pengantar](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program).)


1. Buat file baru bernama index.html, dan simpan kode berikut:
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Hello World!</title>
    </head>
    <body>
        <h1>index.html</h1>
    </body>
    </html>
    ```
2. Di file index.html Anda, masukkan kode ini di baris baru, tepat sebelum tag </html> penutup:
    ```html
    <script>
    const headingKu = document.querySelector('h1');
    headingKu.textContent = 'Hello World!'; // Diganti 'Hello Lort' juga bisa
    </script>
    ```
3. Pastikan file HTML disimpan. Kemudian muat index.html di browser Anda. Anda akan melihat sesuatu seperti ini:
    ![Hello World](https://raw.githubusercontent.com/ksvls/js/gh-pages/img/helloWorld.jpg)

## `Apa Yang Terjadi?`

Heading teks berubah menjadi Hello World! menggunakan JavaScript. Anda melakukan ini dengan menggunakan fungsi yang disebut querySelector() untuk mengambil referensi ke heading Anda, lalu menyimpannya dalam variabel yang disebut headingKu. Ini mirip dengan apa yang kita lakukan menggunakan CSS selectors. Saat Anda ingin melakukan sesuatu pada sebuah elemen, Anda harus memilihnya terlebih dahulu.

Setelah itu, kode menetapkan nilai properti textContent variabel headingKu (yang mewakili konten heading) ke Hello world!.

## Kursus Kilat Dasar JavaScript

Untuk memberi Anda pemahaman yang lebih baik tentang cara kerja JavaScript, mari kita jelaskan beberapa fitur inti bahasa tersebut. Perlu diperhatikan bahwa fitur-fitur ini umum untuk semua bahasa pemrograman. Jika Anda menguasai dasar-dasar ini, Anda juga dapat memulai pengkodean dalam bahasa lain dengan mudah!

## `Variabel`

Variabel adalah wadah yang menyimpan nilai. Anda mulai dengan mendeklarasikan variabel dengan var (kurang disarankan, nanti dijelaskan untuk penjelasannya) atau kata kunci let, diikuti dengan nama yang Anda berikan ke variabel:

```js
let variabelKu;
```

> Catatan: Titik koma (;) di akhir baris menunjukkan tempat pernyataan berakhir. Ini hanya diperlukan jika Anda perlu memisahkan pernyataan dalam satu baris. Namun, beberapa orang percaya bahwa menempatkan titik koma di akhir setiap pernyataan merupakan praktik yang baik. Ada aturan lain tentang kapan Anda harus dan tidak boleh menggunakan titik koma. Untuk lebih jelasnya, lihat [Your Guide to Semicolons in JavaScript](https://news.codecademy.com/your-guide-to-semicolons-in-javascript/).

> Catatan: Anda dapat menamai variabel hampir semua hal, tetapi ada beberapa batasan. ([Lihat bagian ini tentang aturan penamaan]().) Jika Anda tidak yakin, Anda dapat [memeriksa nama variabel Anda](https://mothereff.in/js-variables) untuk melihat apakah itu valid.

> Catatan: JavaScript adalah case-sensitive. Yang berarti variableKu berbeda dengan variabelku. Jika Anda memiliki masalah dalam kode Anda, periksa besar kecil hurufnya!

> Catatan: Untuk detail selengkapnya tentang perbedaan antara var dan let, lihat [Perbedaan antara var dan let]().

Setelah mendeklarasikan variabel, Anda dapat memberinya nilai:
```js
variabelKu = 'Jerry';
```

Selain itu, Anda dapat melakukan kedua operasi ini pada baris yang sama:
```js
let variabelKu = 'Jerry';
```

Anda mengambil nilai dengan memanggil nama variabel:
```js
variabelKu;
```

Setelah menetapkan nilai ke variabel, Anda dapat mengubahnya nanti di kode:
```js
let variabelKu = 'Jerry';
variabelKu = 'Tom';
```

Perhatikan bahwa variabel mungkin memiliki nilai yang memiliki [tipe data]() berbeda:

| Variabel | Penjelasan | Contoh |
|-|-|-|
| [String]() | Ini adalah urutan teks yang dikenal sebagai string. Untuk menunjukkan bahwa nilainya adalah string, apit dengan tanda kutip tunggal. | let variabelKu = 'Jerry'; |
| [Number]() | Ini adalah angka. Angka tidak memiliki tanda kutip di sekitarnya. | let variabelKu = 69; |
| [Boolean]() | Ini adalah nilai Benar / Salah. Kata `true` dan `false` adalah kata kunci khusus yang tidak membutuhkan tanda petik. | let myVariable = true; |
| [Array]() | Ini adalah struktur yang memungkinkan Anda menyimpan banyak nilai dalam satu referensi. | let variabelKu = [1,'Jerry','Tom',69]; Lihat setiap anggota array seperti ini:  variableKu[0], variableKu[1], etc. |
| [Object]() | Ini bisa apa saja. Segala sesuatu di JavaScript adalah sebuah objek dan dapat disimpan dalam sebuah variabel. Ingatlah ini saat Anda belajar. | let variabelKu = document.querySelector('h1'); Semua contoh diatas juga. |

Jadi mengapa kita membutuhkan variabel? Variabel diperlukan untuk melakukan sesuatu yang menarik dalam pemrograman. Jika nilai tidak dapat berubah, maka Anda tidak dapat melakukan sesuatu yang dinamis, seperti mempersonalisasi pesan ucapan atau mengubah gambar yang ditampilkan di galeri gambar.

## `Komentar`

Komentar adalah potongan teks yang dapat ditambahkan bersama dengan kode. Browser mengabaikan teks yang ditandai sebagai komentar. Anda dapat menulis komentar di JavaScript seperti yang Anda bisa di CSS:
```js
/ *
Segala sesuatu di antaranya adalah komentar.
* /
```


Jika komentar Anda tidak berisi jeda baris, itu adalah opsi untuk meletakkannya di belakang dua garis miring seperti ini:
```js
// Ini adalah komentar
```

...sampai disini dulu.
