---
layout : post
date   :  2018-02-10
tags : ["trick", "jekyll"]
categories : jekyll
---

cara mengatasi substr di jekyll kita bisa menggunakan `split`.<br>
Misal kita mau mengambil string `pemograman` dari kalimat `belajar-pemograman`.<br>

kita dapat melakukannya dengan sperti ini.<br>

```
 `{%` assign str = "belajar pemograman" `%}`
  assign splitStr = str | split: '-'
```
dari script di atas kita bisa mendapatkan kata.
`belajar` yang tersimpan di index ke `0`
`pemograman` yang tersimpan di index ke `1`.

```
 splitStr[0] //belajar
 splitStr[1] //pemograman
```

#maridiskusi
