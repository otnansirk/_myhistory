---
layout : post
data   : 2018-10-21,
tags : ["other"]
categories : other
cat-image : cat-other.jpg
---

Dalam contoh ini, kita akan menggunakan domain yang aku  dapatkan dari [hostinger](https://www.hostinger.co.id/){:target="_blank"}.

**1. Setting GitHub Pages**

Kita mulai dengan buka repository github pages, lalu pergi ke menu `setting` .
![]({{site.baseurl}}/images/github-repo.jpg){:.center-box-sadow}

Setelah muncul halaman setting, scroll kebawah bagian `GitHub Pages`.
Dibagian colom `custom domain` masukkan domain sobat.
![]({{site.baseurl}}/images/custom-domain.jpg){:.center-box-sadow}

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
![]({{site.baseurl}}/images/ahost.jpg){:.center-box-sadow}

Cari bagian `CNAME (Alias)` lalu tambahkan `www` pada colom `Host` dan URL pages yang <br>
formatnya `github-username.github.io` di colom `Diarahkan ke`. <br>
Seperti pada gambar no 1 `krisnantobiyuh.github.io`. (ok)

sehingga terlihat seperti ini
![]({{site.baseurl}}/images/cname.jpg){:.center-box-sadow}

Pembaruan DNS ini memerlukan waktu biasanya 1x24 jam+-. tergantung pada providernya (Tempat membeli domain).

Sekian sobat, Feel free to revise this article. 😊







