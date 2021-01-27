---
title: Javascript I
description: Mempelajari dasar-dasar penulisan ES6 - versi baru JavaScript
published: true
date: 2021-01-27T23:26:01.420Z
tags: 
editor: markdown
dateCreated: 2021-01-27T23:04:31.513Z
---

# String & Integer
## Pengantar JavaScript (ES6)
### JavaScript (ES6)
JavaScript (disingkat JS) adalah bahasa skrip yang menjadi element penting dalam pengembangan web. Saat ini, hampir semua situs web menggunakan JS. `JavaScript ES2015 (ES6`), yang akan kita bahas pada pelajaran ini, adalah versi terbaru JS yang menjadi populer karena memungkinkan orang untuk coding dengan lebih efisien.
### Menjalankan Code JS
Pertama, kita akan melihat cara menjalankan (mengeksekusi) code ES6 dan mencetak (menampilkan) rangkaian kata di layar yang disebut console. Saat Anda menulis code <kbd>console.log("Hello World");</kbd>, rangkaian huruf `Hello World` akan di cetak di console.

```js
console.log("hello world");
```
hello world

## console.log()
### console.log()
Sekarang mari kita pelajari cara menulis code JS! <kbd>console.log()</kbd> mencetak rangkaian huruf yang diketik dalam tanda kurung.
Kita menyebut karakter teks, seperti `Hello World`, sebagai `string`. Seperti yang dapat Anda lihat di bawah, Anda harus menggunakan tanda kutip tunggal atau ganda.
```js
console.log("hello world");
console.log('hello world');
```

### Tanda titik koma
Setiap pernyataan harus diakhiri dengan tanda titik koma <kbd>;</kbd>. Tanpa diakhiri titik koma, disebagian besar kasus, code tersebut akan berfungsi secara normal, namun kami sarankan agar anda selalu menyertakanya untuk membiasakan diri bercoding secara rapi dan jelas.

### Cara Memberi Komentar Pada Code
Menulis <kbd>//</kbd> di awal baris akan menjadikan baris tersebut sebagai `komentar`. Artinya, baris ini akan diabaikan saat code dijalankan.
Komentar berguna untuk memberikan catatan dan menjelaskan code Anda, sebagai pengingat pada saat anda mau memperbaruinya ataupun untuk mempermudah tim anda dalam melanjutkan code Anda.
```js
//console.log("hello world");
```

## Kalkulasi (1)
### Angka dan Kalkulasi
Anda juga dapat menggunakan integer (angka) dalam pemrograman. Berbeda dengan string, Anda tidak perlu menggunakan kutipan untuk integer. Integer digunakan untuk melakukan kalkulasi seperti penambahan dan pengurangan. Gunakan <kbd>+</kbd> untuk penambahan dan <kbd>-</kbd> untuk pengurangan.
```js
console.log(3);
console.log(1 + 3);
console.log(2 - 1);
```
3
4
1

### String dan Integer
Seperti contoh di bawah, <kbd>console.log(5 + 2);</kbd> akan mencetak hasil penambahan, yaitu 7. Disisi lain, saat Anda meletakkan <kbd>5 + 2</kbd> dalam tanda kutip, ini akan dicetak sebagai string. Harap diingat bahwa `string` dan `integer` adalah tipe data yang berbeda!
```js
//integer
console.log(5 + 2);

//string
console.log("5 + 2");
```
7
5 + 2

## Kalkulasi (2)
### Pengalian dan Pembagian
Mari kita pelajari cara kalkulasi selain penambahan dan pengurangan! Seperti yang Anda lihat di bawah, `tanda bintang` <kbd>*</kbd> dapat digunakan untuk pengalian dan `garis miring kanan` <kbd>/</kbd> dapat digunakan untuk pembagian. Simbol ini berbeda dari simbol yang digunakan dalam matematika standar, jadi pastikan untuk diingat!
```js
console.log(3 * 5);
console.log(8 / 2);
```
15
4

### Modulo (Sisa Pembagian)
Anda juga dapat menggunakan simbol `persentase` <kbd>%</kbd> untuk mendapatkan `modulo`, sisa setelah pembagian. Ini berguna karena ada banyak cara untuk menggunakan modulo dalam pemrograman!

