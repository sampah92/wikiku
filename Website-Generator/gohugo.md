---
title: Hugo Search Bar
description: menambahkan fitur pencarian pada gohugo
published: true
date: 2020-12-23T18:38:56.949Z
tags: website, gohugo, hugo, fuse.js, mark.js
editor: markdown
dateCreated: 2020-12-22T20:15:32.529Z
---

# instalasi
clone repository modul ke `websitemu/themes/hugo-search-fuse-js`
```
git clone https://github.com/kaushalmodi/hugo-search-fuse-js.git
```
pada `config.toml` tambahkan ini
```
theme = ["hugo-search-fuse-js", "my-theme"]
```
buat file pada `content/` dengan nama file `search.md` dengan cara ketik di terminal
```
hugo new content/search.md
```
edit dan tambahkan ini pada `search.md`
``` yaml
+++
title = "Search"
layout = "search"
outputs = ["html", "json"]
[sitemap]
  priority = 0.1
+++
```
tambahkan identifier pada `config.toml`
