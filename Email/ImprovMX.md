---
title: ImprovMX Email forward dan sender 
description: menggunakan akun Gmail sebagai sender dan forwarder dari custom domain
published: true
date: 2020-12-27T14:33:46.601Z
tags: 
editor: markdown
dateCreated: 2020-12-18T20:26:02.631Z
---

# ImprovMX
ImprovMX dibangun dan diluncurkan oleh `Alexander Tereshkin` sebagai cara untuk mengatur Forward  dan sender email dengan tanpa hosting mandiri ataupun berbayar. ada berbagai fitur premium dari [ImprovMX](https://improvmx.com) dengan harga yang terjangkau, namun yang gratis pun sudah memuaskan.  
# Forward email
Pastikan sudah memiliki custom domain.
- masukan custom domain yang akan diforward ke akun Gmail.
- masukan akun Gmail yang akan digunakan untuk menerima email dari custom domain.
- konfigurasi dan verifikasi kepemilikan domain dengan menginput <kbd>MX records</kbd> dan <kbd>TXT records</kbd> yang telah disediakan [ImprovMX](https://improvmx.com).
- setelah terverifikasi atur alias baru untuk custom email.

# Send email
- Aktifkan [2 faktor autentikasi](https://www.google.com/landing/2step/)
Google akan memverifikasi kepemilikan akun ..
- Pada `select app`pilih <kbd>mail</kbd>  dan pada `select device`pilih <kbd>mac</kbd> lalu `generate`, simpan code untuk tahap beriktnya.
- tambahkan akun custom domain ke akun gmail `gmail --> setting --> account and import`, pilih `add another email address`.
- Masukan alias custom domain pada kolom `Email address`, jangan ceklis `treat as an alias`.
- Kolom `SMTP Server` isi <kbd>smtp.gmail.com</kbd>.
`Username` isi dengan akun gmail yang digunakan.
`Password` isi engan code yang telah di `generate`sebelumnya.
- Google akan mengirim kode ke perangkat mobile untuk verifikasi.

