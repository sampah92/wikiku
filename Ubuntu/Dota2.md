---
title: Dota 2
description: menginstall Dota 2 pada OS Ubuntu
published: true
date: 2020-12-17T12:55:53.697Z
tags: vga, gpu, dota 2
editor: markdown
dateCreated: 2020-12-16T12:34:28.171Z
---

# Konfigurasi
untuk instalasi sama saja sebenarnya, hanya saja ada beberapa setingan yang harus dikonfigurasi.

kasus yang terjadi disini adalah munculnya kode error berikut:
`StartupSubsystems():`
`Panorama requires a full rendersystem, please check your launch options.`

Solusi kasus ini:
`klik kanan pada properties dota 2 di steam` 
`pada startup parameter / launch parameter tambahkan kode berikut :`

<kbd>-safe_mode</kbd>