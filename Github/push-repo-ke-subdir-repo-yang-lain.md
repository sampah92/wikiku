---
title: Push Repo sebagai Subdirecktori
description: menambahkan repo saat ini sebagai subdirektori di repo lain
published: true
date: 2020-12-28T06:26:03.830Z
tags: 
editor: markdown
dateCreated: 2020-12-28T06:26:03.830Z
---

# Konfigurasi
Buat file `.github/workflows/push-to-ra-tools.yml` direpository yang akan dipush ke subdir repo lain.

isi file `.github/workflows/push-to-ra-tools.yml`
```yml
      - name: Pushes to another repository folder
        uses: NoahDragon/action-push-repo-as-subdirectory-in-another-repo@main
        env:
          API_TOKEN_GITHUB: ${{ secrets.API_TOKEN_GITHUB }}
        with:
          dest-repo: 'redwoodedu/tools'
          dest-folder: 'svc`
```
# input 
- `dest-repo`
Nama repositori tujuan, mengikuti pola "USERNAME/REPO_NAME".

- `dest-branch` [opsional]
Nama cabang dalam repositori tujuan. Default adalah utama. Jika tidak ada, CI akan error out.

- folder dest
Nama folder di repo tujuan. Jika tidak ada, akan membuat yang baru. Pastikan nama map sudah benar, jika tidak, semua berkas di bawah map akan ditimpa.

- `commit-message` [opsional]
Pesan commit yang akan digunakan dalam repositori output. Opsional dan default ke "Update from $REPOSITORY_URL@commit".

- `tidak termasuk` [opsional]
Daftar berkas/folder yang dikecualikan di repo tujuan, sehingga tindakan ini tidak akan menimpanya, misalnya berkas konfigurasi. Formatnya adalah titik koma; pisahkan string.
