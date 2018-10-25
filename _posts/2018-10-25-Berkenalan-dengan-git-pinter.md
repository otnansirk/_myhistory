---
layout : post
title  : Berkenalan dengan git-pinter
date   :  2018-10-25,
tags : ["git"]
categories : git
image :
cat-image :
---

Beberapa hari yang lalu saya coba buka-buka repository github dari serior saya
[@akuikialie](https://github.com/akuikialie){:target="_blank"}
dan saya menemukan kembali E-book yang menjadi dasar saya belajar git dengan judul
`git-pinter`. Dari situ lah tulisan ini tercipta. 😄.

> Hallo, [@akuikialie](https://github.com/akuikialie){:target="_blank"}<br>
> *Nama aslinya adalah "Achmad Ali Liesmana", Seorang backend developer di salah satu perusahaan Muslim di surabaya.*

Enaknya pake git bisa membuat versioning di dalam project kerja kita. dan git tidak juga digunakan untuk versioning source code.
Tapi, juga bisa untuk kalian para `mahasiswa` yang sedang melakukan tugas panjang. seperti `scripsi`. <br>
Misal saja kita membuat laporan di dalam MS-Word, kita bisa memanfaatkan `git` ini untuk versioning scripsi kita,
Jadi tidak perlu takut data hilang, kedelete dll. Karena git akan menyimpan perubahan-perubahan walau hanya satu space saja.

Untuk teori seperti apa itu git ?<br>
Dan lain-lainnya bisa di baca detail di google 😄 atau bisa juga di [git-pinter](https://github.com/akuikialie/git-pinter/blob/master/git-pinter.pdf){:target="_blank"}.(mastahku)

Oke, lanjut kepraktek.
 **Install git**
 * *Windows* <br>
   Dowload git [disini](https://git-scm.com/download/win){:target="_blank"}. setelah itu jalankan file .exe lalu ikuti langkah-langkahnya sampai selesai.

* *Linux* <br>
  Jalankan perintah berikut
    ```
    $ sudo apt update
    $ sudo apt install git
    ```

**Setup git** <br>
    Setelah selesai installnya kita perlu mengatur username dan email yang nantiya akan menjadi identitas
    kita saat melakukan aktivitas pada git.

```
$ git config --global user.name "krisnanto"
$ git config --global user.email "krisnantobiyuh@gmail.com"
```

**Menggunakan git**

* *Inisialisasi - membuat repository baru* <br>
  *git-init* <br>
  Seblumnya kita masuk dulu ke folder yang akan kita gunakan untuk menyimpan file-file source code kita.
```
krisnantobiyuh@kris:~/Document/git-pinter$
```

  Lalu kita inisialisasi folder `git-pinter`
  ```
  krisnantobiyuh@kris:~/Document/git-pinter$ git init
  ```
![]({{site.baseurl}}/images/git-init.jpg){:.left-box-sadow}
  Sampai proses ini kita akan melihat `/.git` didalam folder `git-pinter`. menandakan proses `git init` successfuly.

* *Membuat dan melihat perubahan* <br>
  *git-status* <br>
  Coba buat kita `first-file.txt` dengan `notepad`. Ketikkan nama kalian di dalamnya.
    ```
    Nama : Krisnanto
    ```
    Setelah itu save di folder `git-pinter`.
    Masuk lagi ke terminal dan ketikkan
     ```
    krisnantobiyuh@kris:~/Document/git-pinter$ git status
    ```
    Kita akan melihat perubahannya seperti ini.
    ![]({{site.baseurl}}/images/git-status.jpg){:.left-box-sadow}
    Menandakan ada perubahan yang belum kita `add` kedalam index.


* *Menambahkan perubahan kedalam index* <br>
  *git-add* <br>
    ```
    krisnantobiyuh@kris:~/Document/git-pinter$ git add .
    ```

    Masuk lagi ke terminal dan ketikkan
    ```
    krisnantobiyuh@kris:~/Document/git-pinter$ git status
    ```
    Kita akan melihat perubahannya seperti ini.
    ![]({{site.baseurl}}/images/git-status-after-add.jpg){:.left-box-sadow}
    menandakan file perubahan sudah di `add` dan siap di `commit`.

* *Menyimpan perubahan ke repository* <br>
  *git-commit* <br>
    Menyimpan perubahan yang sudah kita `add` ke dalam repository kita.
    ```
    krisnantobiyuh@kris:~/Document/git-pinter$ git commit -m "first commit" .
    ```

* *Membuat remote repository* <br>
  *git remote* <br>
    Buat sebuah sepository di github dengan nama `git-pinter`. setelah itu kita add remote.
    ```
    git remote add origin https://github.com/username-github-kalian/git-pinter.git
    ```
    Menambahkan remote repository ke dalam projevt git kita.

* *Megirim perubahan* <br>
  *git-push* <br>
    Menyimpan/mengirimkan perubahan yang sudah kita `commit` ke remote repository kita.
    ```
    krisnantobiyuh@kris:~/Document/git-pinter$ git push origin master .
    ```
    Perubahan yang berada dilocal kita sudah terkirim dan tersimpan.

    Untuk melihat coba lakukan check status `git-status`.
    ```
    krisnantobiyuh@kris:~/Document/git-pinter$ git status
    ```
    Muncul `nothing to commit, working tree clean`. menandakan tidak ada perubahan didalam working tree kita.

  Jangan ragu koreksi tulsan ini jika ada yang salah. #maridiskusi. 😉



