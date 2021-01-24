---
title: Python III
description: Pada pelajaran ini, kita akan belajar bagaimana cara menggunakan function dan module.
published: true
date: 2021-01-24T17:37:18.588Z
tags: 
editor: markdown
dateCreated: 2021-01-24T17:24:54.095Z
---

# Mari Mulai
Pada pelajaran ini, kita akan belajar bagaimana cara menggunakan `function` dan `module`.
Untuk membuat pelajaran ini menjadi lebih menyenangkan,
mari kita mempelajarinya sambil membuat permainan Batu Kertas Gunting.

# Function
## Function
Pertama-tama, mari kita lihat bagaimana `function` bekerja dalam Python. Function adalah bagian dari code yang menjalankan tugas tertentu. `print` adalah salah satu contoh function, yang memudahkan Anda untuk mencetak teks tanpa perlu untuk menulis banyak code.

### Lebih lanjut tentang function
Seperti `print`, ada banyak function yang sudah tersedia di Python yang dapat membuat coding lebih mudah. Jika tertarik, Anda juga dapat membuat function Anda sendiri.

### Mendefinisikan Function
Mari belajar bagaimana cara mendefinisikan function yang sederhana.
Sintaksis untuk mendefinisikan function adalah sebagai berikut:
`def function_name():`
Jangan lupa untuk mengindentasi code didalam function.
```python
def function_name():
___#Code 
#gunakan indentasi
```
Contoh
```python
def gree():
		print("halo")
```
### Memanggil Function
Function tidak akan dijalankan hanya dengan mendefinisikannya, Anda perlu `memanggil` function untuk menjalankan code didalamnya. Untuk memanggil sebuah function, Anda cukup menulis `function_name()`. Perlu diingat bahwa function hanya dapat dipanggil setelah Anda mendefinisikannya.
```python
def greet():
		print("halo")

greet()	# Memanggil function

#Hasil: halo
```
## Argument dan Parameter
### Apa Itu Argument?
Anda dapat memberikan nilai ke sebuah function ketika Anda memanggilnya. Nilai ini disebut `argument` dan dapat digunakan berulang kali di dalam sebuah function. Dengan menggunakan argument, Anda dapat membuat sebuah function untuk me-return nilai yang berbeda berdasarkan argument yang Anda berikan.

### Function dengan Argument
Untuk memberikan `argument` ke sebuah function, function harus mempunyai variable untuk menerimanya, variable ini di sebut `parameter`. Pada contoh di bawah, function <kbd>greet</kbd> memiliki parameter <kbd>name</kbd> untuk menerima sebuah argument.
```python
def function_name(parameter):
		              # variabel yang dibutuhkan
    #Code
```
```python
def greet(name):
		print("halo" + name)
```
### Memberikan Argument ke Sebuah Function
Kita bisa memberikan argument dengan memanggil sebuah function dengan: <kbd>function_name(argument)</kbd>. Saat function dipanggil, `argument` yang diberikan akan ditentukan ke `parameter` untuk digunakan di dalam function.
```python
def greet(name): # Parameter name
		print("halo" + name)
    
greet("john") # john diberikan ke parameter name
greet("kate")

#Hasil: halo john
#Hasil: halo kate
```
### Scope
Variable mempunyai `scope`, sesuatu yang merujuk ke rentang tertentu dimana variable dapat diakses. Scope dari parameter dan variable yang di definisikan didalam sebuah function akan terbatas pada function tersebut. Maka dari itu, mereka tidak dapat digunakan diluar function itu.
```python
def greet(name): # Parameter name
		print(name) # hanya dapat digunakan didalam function ini
    
print(name) <---- # diluar scope

# ERROR! - Variable name tidak dapat digunakan diluar function
```