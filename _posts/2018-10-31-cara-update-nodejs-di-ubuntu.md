---
layout : post
title  : Cara update nodejs di ubuntu
date   : 2018-10-31,
tags : ["nodejs"]
categories : nodejs
image : "cat-nodejs.jpg"
cat-image : "cat-nodejs.jpg"
---

Udah beberapa hari gak nulis :D. Kali ini mau share riangan aja sih. Gimana cara update nodejs di ubuntu.
Ya sekalian biar aku punya dokumentasi sendiri :D.

Mulai aja ya. sebelumnya nodejs yang aku punya `v4.2.6` dan npmnya `v3.5.2`.<br>
pertama lakukan update package.
```
$ sudo apt-get update
```
dan pastikan `curl` sudah terinstall. jika belum install dulu.
```
$ sudo agt-get install curl
```
Setelah selesai, kita perlu download dan menjalankan script install yang sudah disediakan oleh NodeSource.

```
$ curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
```
Mungkin ini akan memakan waktu lebih lama dari sebelumnya. setelah download dan sets up repository dari NodeSource selesai.
Jalankan `apt-get update` lagi. lalu install nodejs.

```
$ sudo apt-get install nodejs
```

Ini akan menginstall nodejs `v8.12.0` (pada saat dokumentasi ini ditulis).
Jika device sobat sudah terintall nodejs, tenang.
Karena script ini akan meng-upgrade nodejs yang sudah ada.

untuk memastikan nya update berhasil. Coba cek
```
$ node -v
```

Jangan sungkan bertanya ya. #maridiskusi

