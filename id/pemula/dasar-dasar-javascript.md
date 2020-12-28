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
    const headingKu = document.querySelector('h1')
    headingKu.textContent = 'Hello World!' // Diganti 'Hello Lort' juga bisa
    </script>
    ```
3. Pastikan file HTML disimpan. Kemudian muat index.html di browser Anda. Anda akan melihat sesuatu seperti ini:
    ![Hello World](https://raw.githubusercontent.com/ksvls/js/gh-pages/img/helloWorld.jpg)

## `Apa Yang Terjadi?`

Heading teks berubah menjadi Hello World! menggunakan JavaScript. Anda melakukan ini dengan menggunakan fungsi yang disebut querySelector() untuk mengambil referensi ke heading Anda, lalu menyimpannya dalam variabel yang disebut headingKu. Ini mirip dengan apa yang kita lakukan menggunakan CSS selectors. Saat Anda ingin melakukan sesuatu pada sebuah elemen, Anda harus memilihnya terlebih dahulu.

Setelah itu, kode menetapkan nilai properti textContent variabel headingKu (yang mewakili konten heading) ke Hello world!.
