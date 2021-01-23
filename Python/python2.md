---
title: Python II
description: kita akan belajar bagaimana mengelola kumpulan data dan bekerja dengan loop.
published: true
date: 2021-01-23T13:35:56.980Z
tags: 
editor: markdown
dateCreated: 2021-01-23T06:51:27.942Z
---

# Mari Mulai
Pada pelajaran ini, kita akan belajar bagaimana mengelola kumpulan data dan bekerja dengan loop.
Kita juga akan memperbarui aplikasi belanja dengan pengetahuan baru ini.
Tidak akan sesulit kedengarannya, kok. Santai!
# Menyusun Data
## List
### Menyusun Data
Mari belajar bagaimana mengelola sekelompok data dengan satu variable. Ketika ada daftar nama-nama makanan, sebagai contoh, tidak efisien untuk menamainya dengan variable terpisah, seperti `food1`, `food2`, `food3`. Akan lebih baik untuk mempunyai variable `foods` untuk mengelola keseluruhan daftar tersebut.
> **Variabel** Mengelola data secara **mandiri**
{.is-info}
```mermaid
graph LR
pasta --> food1
```
```mermaid
graph LR
gulai --> food2
```
```mermaid
graph LR
sushi --> food3
```
> **List** Mengelola sekelompok data secara **bersamaan**
{.is-info}
```mermaid
 classDiagram
foods <|-- data
class data{
    pasta
    gulai
    sushi
}
```
### List (Daftar)
Tipe data `list` memungkinkan Anda untuk mengelola sekelompok data sekaligus. Anda dapat membuat list sebagai berikut: `[element1, element2, ...]`. Setiap nilai di dalam list disebut `element`.
Dengan menggunakan list, Anda dapat mengelola banyak string dan integer dalam satu grup.

Membuat List
```
[element1, element2, element3]
# Pisahakan element dengan koma
```
Penggunaan
```python
# List dari beberapa string
["pasta", "gulai", "sushi"]

# List dari beberapa integer
[1, 2, 3, 5, 8, 13, 21]

# List dari item gabungan
[["apel", "pisang", 200, 300]
```
### Menetapkan List ke Variable
Seperti integer dan string, Anda dapat menentukan list ke dalam satu variable. Sesuai norma penamaan yang berlaku, nama variable bersifat plural, seperti `foods`, karena variable akan mengandung banyak element.

```python
foods = ["pasta", "gulai", "sushi"]  # foods = nama variabel
print(foods)

#Hasil: ["pasta", "gulai", "sushi"]
# List dicetak sebagaimana adanya
```

### Menentukan Element dalam List
Setiap element list dinomori `0, 1, 2, ....`
Ini disebut `nomor indeks`. Nomor indeks dimulai dari `0`. Anda bisa mendapatkan element individual dengan menulis `list[index]`.

Index
```python
["pasta", "gulai", "sushi]
	  0				1					2

# dimulai dari index 0
```
```python
foods = ["pasta", "gulai", "sushi"]
print("saya suka " + foods[2]) # Mengambil element menggunakan nomor index

# Element dengan index 2 dicetak
# Hasil: Saya suka sushi
```
## Memperbarui dan Menambah Element-Element List
### Memperbarui Element Pada List
Mari kita mencoba untuk memperbarui element pada list.
Ini dapat dilakukan dengan menulis `list[index] = nilai`.
```python
foods = ["pasta", "gulai", "sushi"] 
foods[1] = "pizza" # Memperbarui element index 1 
print(foods)

#Hasil: ["pasta", "gulai", "sushi"]
# Element di index 1 diperbarui
```
### Menambah Element Pada List
Anda juga dapat menambah element pada list.
Dengan menulis `list.append(nilai)`, Anda dapat menambahkan element baru pada akhir sebuah list.
```python
foods = ["pasta", "gulai", "sushi"] 
foods.append("pizza") # Menambah element ke akhir list 
print(foods)

#Hasil: ["pasta", "gulai", "sushi", "pizza]
# Sebuah element ditambahkan
```

## Loop for
### Mencetak Semua Element
Jika Anda ingin mencetak semua element pada list, tidak efisien untuk mengulang code yang sama seperti contoh pada gambar di sebelah kiri.
Anda dapat menggunakan `loop for` untuk memudahkan Anda mencetak semua element.
```python
foods = ["pasta", "gulai", "sushi"]
print("Saya suka " + foods[1])
print("Saya suka " + foods[2])
print("Saya suka " + foods[3])
# Mencetak satu per satu tidak efisien

#Hasil:
#Saya suka pasta
#Saya suka gulai
#Saya suka sushi
```

### Loop for
Loop `for` memudahkan Anda untuk memproses setiap element pada list dengan temporary variable (variable sementara) dan mengaplikasikan code yang sama.
Pada contoh di bawah, tiap element pada variable `foods` disimpan pada variable sementara, yaitu `food` dan dicetak.
```python
foods = ["pasta", "gulai", "sushi"]
for food in foods:  #food = temporary variable    
		print("Saya suka " + food
    
#Hasil:
#Saya suka pasta
#Saya suka gulai
#Saya suka sushi
```