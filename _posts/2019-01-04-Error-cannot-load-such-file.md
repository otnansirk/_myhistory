---
layout : post
title  : Error cannot load such file -- bundler pada saat check version jekyll
date   : 2019-01-04,
tags : ["jekyll","error"]
categories : jekyll
---

Pernah kalian mengalami error pada jekyll ?.
Setelah selesai instalasi. Ternyata aku mendapat error saat melakukan check version pada jekyll.

ini isi error nya. 
```
Traceback (most recent call last):
        5: from /home/hrmlabs/gems/bin/jekyll:23:in `<main>'
        4: from /home/hrmlabs/gems/bin/jekyll:23:in `load'
        3: from /home/hrmlabs/gems/gems/jekyll-3.8.5/exe/jekyll:11:in `<top (required)>'
        2: from /home/hrmlabs/gems/gems/jekyll-3.8.5/lib/jekyll/plugin_manager.rb:48:in `require_from_bundler'
        1: from /usr/lib/ruby/2.5.0/rubygems/core_ext/kernel_require.rb:59:in `require'
/usr/lib/ruby/2.5.0/rubygems/core_ext/kernel_require.rb:59:in `require': cannot load such file -- bundler (LoadError)
```

dan error ini terpecahkan hanya dengan mengupdate bundle nya yaitu.
```
$ bundle update
```

Hanya dengan satu kali exsekusi `bundle update` masalah di atas bisa terselesaikan. :D

 #maridiskusi

