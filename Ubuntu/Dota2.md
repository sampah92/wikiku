---
title: Dota 2
description: menginstall Dota 2 pada OS Ubuntu 20.04
published: true
date: 2020-12-22T14:09:01.614Z
tags: vga, gpu, dota 2, game, ubuntu 20.04
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

```
-safe_mode
```