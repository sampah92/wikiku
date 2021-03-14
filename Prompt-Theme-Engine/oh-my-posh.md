---
title: Oh-my-posh
description: A prompt theme engine for any shell
published: true
date: 2021-03-14T22:41:22.586Z
tags: 
editor: markdown
dateCreated: 2021-03-14T22:41:22.586Z
---

# Pendahuluan
[Oh-my-posh](https://ohmyposh.dev/) merupakan salah satu prompt theme engine terbaik dengan berbagai fitur dan dapat dijalankan hampir di sistem operasi yang ada saat ini.

# Kelebihan
Tidak peduli shell mana yang Anda gunakan, atau bahkan berapa banyak, Anda dapat membawa konfigurasi dari satu shell dan / atau mesin ke yang lain untuk prompt yang sama di mana pun Anda bekerja.

# Petunjuk Instalasi
tidak usah menulis panjang lebar [disini](https://ohmyposh.dev/docs/installation) sudah ada.

# Theme
Dari beberapa tema yang ada, saya lebih tertarik pada [DarkBlood](https://github.com/JanDeDobbeleer/oh-my-posh/blob/main/themes/darkblood.omp.json). beberapa eleman pada DarkBlood sudah saya sesuaikan berdasarkan keinginan saya.

berikut konfigurasi yang sudah saya modifikasi:

```json
{
  "$schema": "https://raw.githubusercontent.com/JanDeDobbeleer/oh-my-posh/main/themes/schema.json",
  "blocks": [
    {
      "type": "prompt",
      "alignment": "left",
      "segments": [
        {
          "type": "session",
          "style": "plain",
          "foreground": "#54B78C",
          "properties": {
            "user_info_separator": "",
            "display_host": false,
            "prefix": "<#1F858D>┌────\uE0B7</>",
            "postfix": "<#1F858D></>"
          }
        },
        
        {
          "type": "path",
          "style": "powerline",
          "foreground": "#E8D251",
          "properties": {
            "style": "folder",
            "mixed_threshold": 2,
            "home_icon": "\uf015",
            "prefix": "<#1F858D>─</>",
            "postfix": "<#1F858D></>"
          }
        },
        {
          "type": "git",
          "style": "plain",
          "foreground": "#D0666F",
          "properties": {
            "display_stash_count": true,
            "display_upstream_icon": true,
            "display_status": true,
            "status_colors_enabled": true,
            "color_background": false,
            "local_changes_color": "#ffeb3b",
            "working_color": "#E84855",
            "staging_color": "#2FDA4E",
            "ahead_color": "#2EC4B6",
            "behind_color": "#8A4FFF",
            "prefix": "<#1F858D>─</>",
            "postfix": "<#1F858D></>"
          }
        },
        {
          "type": "root",
          "style": "plain",
          "foreground": "#AB4E3D",
          "properties": {
            "prefix": "<#235f35>[</>",
            "postfix": "<#235f35>]</>"
          }
        },
        {
          "type": "exit",
          "style": "diamond",
          "foreground": "#ffffff",
          "background": "#2e9599",
          "leading_diamond": "",
          "trailing_diamond": "\uE0B4",
          "properties": {
            "display_exit_code": false,
            "always_enabled": true,
            "error_color": "#f1184c",
            "color_background": true,
            "prefix": "<transparent></> \uE23A"
          }
        }
      ]
    },
    {
      "type": "prompt",
      "alignment": "right",
      "segments": [
        {
          "type": "node",
          "style": "plain",
          "foreground": "#6CA35E",
          "properties": {
            "prefix": " <#1F858D>  \uE718</> ",
            "postfix": "<#1F858D> </>"
          }
        },
        {
          "type": "python",
          "style": "diamond",
          "foreground": "#96E072",
          "background": "#2f2f2f",
          "properties": {
            "prefix": " \uE235 ",
            "postfix": "<#7a7a7a> \ue0b3</>"
          }
        },
        {
          "type": "dotnet",
          "style": "diamond",
          "foreground": "#3891A6",
          "background": "#2f2f2f",
          "properties": {
            "prefix": " \uE77F ",
            "postfix": "<#7a7a7a> \ue0b3</>"
          }
        }
      ]
    },
    {
     "type": "newline"
    },
    {
      "type": "prompt",
      "alignment": "left",
      "segments": [       
        {
          "type": "text",
          "style": "plain",
          "foreground": "#54B78C",
          "properties": {
            "prefix": "<#1F858D>└─</>",
            "postfix": "<#54B78C>\u276F</>",
            "text": "\u276F"
          }
        }
      ]
    }
  ],
  "final_space": true
}
```

## Cara menggunakan tema ini
- install [window terminal](https://www.microsoft.com/en-us/p/windows-terminal/9n0dx20hk701).
- install font [MesloLGM NF](https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/Meslo.zip) atau [Cascadia Code LP](https://github.com/microsoft/cascadia-code/releases) terlebih dahulu.
- buka window terminal, klik kanan pada `toolbar` dan pilih `setting`.
```json
    "profiles":
    {
        "defaults":
        {
            // Put settings here that you want to apply to all profiles.
            "fontFace": "MesloLGM NF", <----- ubah font menjadi cascadia atau meslo
            "fontSize": 10
            
        },
        "list":
        [
            {
                // Make changes here to the powershell.exe profile.
                "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
                "name": "Windows PowerShell",
                "commandline": "powershell.exe",
                "fontFace": "MesloLGM NF", <----- ubah font menjadi cascadia atau meslo
                "hidden": false
                
            },
      
          ----------------> sebaiknya semua "fontface" diganti <--------------------
```
- sekian
