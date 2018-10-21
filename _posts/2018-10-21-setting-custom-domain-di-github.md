---
layout : post
data   : 2018-10-21,
tags : ["other"]
categories : other
cat-image : cat-other.jpg
---

Dalam contoh ini, kita akan menggunakan domain yang aku dapatkan dari [hostinger](https://www.hostinger.co.id/){:target="_blank"}.

**1. Setting GitHub Pages**

Kita mulai dengan buka repository github pages, lalu pergi ke menu `setting` .
<center>
<img src="{{site.baseurl}}/images/1/github-repo.png" width="650" style="box-shadow: 0 0 5px #d9d9d9, 0 0 15px #999999">
<br> Gambar 3
</center>

Setelah muncul halaman setting, scroll kebawah bagian `GitHub Pages`.
Dibagian colom `custom domain` masukkan domain sobat.
<center>
<img src="{{site.baseurl}}/images/1/custom-domain.png" width="650" style="box-shadow: 0 0 5px #d9d9d9, 0 0 15px #999999">
<br> Gambar 4
</center>

**2. Setting Domain**

Masuk ke akun hostinger, lalu klik `kelola` yang terdapat di list domain.
Setelah masuk kedalam halaman kelola domain pilih tab `DNS ZONE`.

Cari bagian `A(Host)` lalu tambahkan `@` pada colom `Host`, dan IP-Address berikut di colom `Diarahkan ke`.
satu persatu.

{% highlight php %}
"185.199.108.153".
"185.199.109.153".
"185.199.110.153".
"185.199.111.153".
{% endhighlight %}

sehingga terlihat seperti ini
<center>
<img src="{{site.baseurl}}/images/1/Ahost.png" width="650" style="box-shadow: 0 0 5px #d9d9d9, 0 0 15px #999999">
<br> Gambar 1
</center>

Cari bagian `CNAME (Alias)` lalu tambahkan `www` pada colom `Host` dan URL pages yang <br>
formatnya `github-username.github.io` di colom `Diarahkan ke`. <br>
Seperti pada gambar no 1 `krisnantobiyuh.github.io`

sehingga terlihat seperti ini
<center>
<img src="{{site.baseurl}}/images/1/cname.png" width="650" style="box-shadow: 0 0 5px #d9d9d9, 0 0 15px #999999">
<br> Gambar 2
</center>

Pembaruan DNS ini memerlukan waktu biasanya 1x24 jam+-. tergantung pada providernya (Tempat membeli domain).

Sekian sobat, Feel free to revise this article. 😊







