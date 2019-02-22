---
layout : default
date   :  2018-10-20
tags : ["mongodb"]
categories : mongodb
---

Menghapus field dari document. Kenapa harus dihapus fieldnya? kenapa tidak memberi value
`null`, `[]`, atau `""` saja.
Sebenernya memberi value tersbut tidak jadi masalah, tapi terkadang kita perlu menghapus
field dari document karena kebutuhan tertentu.
Lalu bagaimana caranya. oke langsung saja

Kita punya data `personal detail` sebagai berikut.

{% highlight json %}
"personalDetail" : {
    "name" : "krisnanto",
    "address" : [
        {
            "_id" : ObjectId("5bc834a4d068620b030c5642"),
            "number" : 12,
            "text" : "Orchard Hotel"
        },
        {
            "_id" : ObjectId("5bc834a4d068620b030c5642"),
            "number" : 12,
            "text" : "Village Hotel Changi"
        }
    ]
},
{% endhighlight %}

Dan casenya adalah kita mau menghapus field `address`.

Berikut query untuk menghapus filed. Gunakan `$unset`:

{% highlight mongodb %}
db.collection.update(
   {"personalDetail.name" : "krisnanto" },
   {"$unset" : {"personalDetail.address" : 1}}
)
{% endhighlight %}

Setelah query dieksekusi, seharusnya data akan terlihat seperti ini :
{% highlight json %}
"personalDetail" : {
    "name" : "krisnanto"
},
{% endhighlight %}


