---
title: Python IV
description: mengenal konsep penting di Python yaitu class dan instance
published: true
date: 2021-01-27T10:50:27.662Z
tags: 
editor: markdown
dateCreated: 2021-01-27T10:50:27.662Z
---

# Class dan Instance
## Gambaran
### Pemahaman Produk
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
