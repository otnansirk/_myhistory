---
layout : post
title  : ERROR: Failed to build gem native extension
date   : 2019-02-09,
tags : ["jekyll","error"]
categories : jekyll
---

Jika mengalami error `ERROR: Failed to build gem native extension` saat menjalankan `gem install jekyll bundler` ?
Mungkin kita belum menginstall ruby-dev.

Coba install ruby-dev dulu dengan command. 
```
$ apt-get install ruby-dev
```

setelah itu coba kita lakukan lagi install jekyll bundler dengan command.
```
$ gem install jekyll bundler
```

 #maridiskusi

