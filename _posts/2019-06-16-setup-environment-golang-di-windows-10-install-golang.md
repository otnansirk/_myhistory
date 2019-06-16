---
layout : post
title: Setup environment GoLang di windows 10 -  Install Golang
date   :  2019-06-16
tags : ["trick", "php"]
categories : golang
cat-image : "cat-golang.jpg"
---

Pada saat ini GoLang adalah bahasa yang paling banyak dibicarakan di beberapa forum dan juga kalangan programmer.

## **Download dan Intall**
Oke langsung saja hal pertama kali tentunya download dulu ya.
bisa download [disini](https://golang.org/dl/). Pilih saja sesuai dengan arsitektur windows kalian.

setelah selesai kita download. <br>
langsung aja install golang nya. seperti biasa di windows tinggal next-next aja 😁  .

## **Setting Environment Variable**
Setelah selesai install biasanya folder default nya di `C:\Go`.

Buka `Environment Variable`. agar lebih cepat search aja di windows cortana.

![]({{site.baseurl}}/images/env-search.png){:.center-box-sadow}
Pilih `Environment Variable`
![]({{site.baseurl}}/images/system-property.png){:.center-box-sadow}

Copy `GOPATH` ke environment variable. jadi nanti semua project `Go` kita letakkan dalam folder ini.
![]({{site.baseurl}}/images/new-system-variable.png){:.center-box-sadow}

Disini saya akan meletakkan project `Go` di `D:\krisnantobi\GoLang-project` maka saya akan setting seperti ini
![]({{site.baseurl}}/images/system-variable-add.png){:.center-box-sadow}

setelah semua selesai jangan lupa `save`.

## **Check Golang Env**
Setelah selesai setting environment coba jalankan `go env` di terminal (cmd) pada windows <br>
jika berhasil maka akan muncul seperti ini
![]({{site.baseurl}}/images/go-env.png){:.center-box-sadow}

## **Test Hello Word**
coba buat foler `helloWord` di dalam direktori `GOPATH` yang sudah kita setting. <br>
punya saya disini `D:\krisnantobi\GoLang-project`.<br>
setelah itu tambahkan file `hello.go` dan ketikkan code berikut <br>
```
package main

import ("fmt")

func main() {
    fmt.Printf("Hello word\n")
}
```
lalu jalankan perintah berikut di terminal (cmd) tepat di direktori root project. <br>
punya saya berapi di `D:\krisnantobi\GoLang-project\helloWord` <br>
```
$go run hello.go
```
<br>
jika settingan yang kita buat success maka seharusnya kita bisa lihat string `Hello word` setelah kita run perintah di atas.
<br>
sumber : [https://golang.org/doc/install](https://golang.org/doc/install)


Jangan lupa #maridiskusi 😁


