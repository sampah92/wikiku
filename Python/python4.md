---
title: Python IV
description: mengenal konsep penting di Python yaitu class dan instance
published: true
date: 2021-01-27T10:55:48.816Z
tags: 
editor: markdown
dateCreated: 2021-01-27T10:50:27.662Z
---

# Class dan Instance
## Gambaran
Kita akan mempelajari `class`. Ini adalah ilmu yang sangat penting dalam Python, jadi mari kita mempelajarinya dengan sungguh-sungguh!
> Anda dapat melihat ada item-item menu berbeda.
Kita akan memperlakukan tiap item menu sebagai tipe `object` yang sama, ini akan memudahkan kita untuk mengelola itemnya dengan nomor.
### Pemahaman Produk
Pertama, mari kita lihat bagaimana aplikasi pemesanan makanan akan bekerja. Saat berjalan, program akan menerima nomor item menu dan kuantitasnya sesuai dengan yang dimasukkan pengguna.
## Definisi Class
```mermaid
 classDiagram
			Menu1 --|> Deskripsi
       Menu2 --|> Deskripsi
      class Deskripsi{
          Setiap item 
          menu memiliki 
          'nama' dan 'harga'
      }
      class Menu1{
          - Nama: Kue_Coklat
          - harga: $4
      }
      class Menu2{
          - Nama: Roti_Lapis
          - harga: $5
      }
