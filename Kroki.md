---
title: Kroki
description: Membuat diagram dari deskripsi tekstual!
published: true
date: 2021-02-06T13:49:09.935Z
tags: 
editor: markdown
dateCreated: 2021-02-06T13:25:35.819Z
---

# Pendahuluan
[Kroki](https://kroki.io/) menyediakan API terpadu dengan dukungan antara lain:
- [BlockDiag](http://blockdiag.com/)
- [SeqDiag](http://blockdiag.com/en/seqdiag/index.html)
- [ActDiag](http://blockdiag.com/en/actdiag/index.html)
- [NwDiag](http://blockdiag.com/en/nwdiag/)
- [PacketDiag](http://blockdiag.com/en/packetdiag/index.html)
- [RackDiag](http://blockdiag.com/en/nwdiag/rackdiag-examples.html)
- [BPMN](https://bpmn.io/)
- Bytefield
- [C4 (dengan PlantUML](https://c4model.com/)
- [Ditaa](https://plantuml.com/ditaa)
- [Erd](https://www.smartdraw.com/entity-relationship-diagram/)
- [Excalidraw](https://excalidraw.com/)
- [GraphViz](https://graphviz.org/)
- [Mermaid](https://mermaid-js.github.io/mermaid/#/)
- [Nomnoml](https://rstudio.github.io/nomnoml/)
- [PlantUML](https://plantuml.com/)
- [SvgBob](https://ivanceras.github.io/content/Svgbob/Specification.html)
- [UMLet](https://www.umlet.com/)
- [Vega](https://vega.github.io/vega/)
- [Vega-Lite](https://vega.github.io/vega-lite/docs/selection.html)

dan banyak lagi yang akan datang!

# Fitur
> `Siap digunakan`
<font size="2"> Pustaka diagram ditulis dalam berbagai bahasa: Haskell, Python, JavaScript, Go, PHP, Java... beberapa juga memiliki ikatan C.</font>
{.is-success}


> Sederhana
<font size="2">Kroki menyediakan API terpadu untuk semua library diagram. Pelajari sekali gunakan diagram di mana saja!</font>
{.is-success}


> Sumber gratis &amp; terbuka
<font size="2">Semua kode tersedia di GitHub dan tujuan kami adalah untuk menyediakan Kroki sebagai layanan gratis.</font>
{.is-success}


> Cepat
<font size="2">Dibangun menggunakan arsitektur modern, Kroki menawarkan performa yang luar biasa.</font>
{.is-success}



# Diagram Tipe
| Diagram Type     | png | svg | jpeg | pdf | base64 |
|------------------|-----|-----|------|-----|--------|
| BlockDiag        | ✔️   | ✔️   |      | ✔️   | ️       |
| BPMN             | ️    | ✔️   |      | ️    | ️       |
| Bytefield        | ️    | ✔️   |      | ️    | ️       |
| SeqDiag          | ✔️   | ✔️   |      | ✔️   | ️       |
| ActDiag          | ✔️   | ✔️   |      | ✔️   | ️       |
| NwDiag           | ✔️   | ✔️   |      | ✔️   | ️       |
| PacketDiag       | ✔️   | ✔️   |      | ✔️   | ️       |
| RackDiag         | ✔️   | ✔️   |      | ✔️   | ️       |
| C4 with PlantUML | ✔️   | ✔️   | ✔️    | ️    | ✔️      |
| Ditaa            | ✔️   | ✔️   |      | ️    | ️       |
| Erd              | ✔️   | ✔️   | ✔️    | ✔️   | ️       |
| Excalidraw       | ️    | ✔️   | ️     | ️    | ️       |
| GraphViz         | ✔️   | ✔️   | ✔️    | ✔️   |        |
| Mermaid          |     | ✔️   |      |     |        |
| Nomnoml          | ️    | ✔️   | ️     |     |        |
| PlantUML         | ✔️   | ✔️   | ✔️    | ️    | ✔️      |
| Svgbob           | ️    | ✔️   | ️     | ️    |        |
| UMlet            | ✔️   | ✔️   | ✔️    | ️    |        |
| Vega             | ✔️   | ✔️   |      | ✔️   | ️       |
| Vega-Lite        | ✔️   | ✔️   |      | ✔️   | ️       |
| WaveDrom         |     | ✔️   |      |     | ️       |

# Penggunaan
<p> ```kroki
<br>mermaid

graph TD
  A[ Anyone ] -->|Can help | B( Go to github.com/yuzutech/kroki )
  B --> C{ How to contribute? }
  C --> D[ Reporting bugs ]
  C --> E[ Sharing ideas ]
  C --> F[ Advocating ]
<p>```</p>
<br>

- hasil
```kroki
mermaid

graph TD
  A[ Anyone ] -->|Can help | B( Go to github.com/yuzutech/kroki )
  B --> C{ How to contribute? }
  C --> D[ Reporting bugs ]
  C --> E[ Sharing ideas ]
  C --> F[ Advocating ]
```