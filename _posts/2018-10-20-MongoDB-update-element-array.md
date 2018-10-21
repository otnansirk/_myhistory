---
layout : post
data   :  2018-10-20
tags : ["mongodb"]
categories : mongodb
cat-image : "cat-mongodb.jpg"
---

Bagaimana cara update data berdasarkan filter _id di dalam setiap element array ?
semisal kita punya data `personal detail` sebagai berikut.

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

Dan casenya adalah kita mau mengedit address dengan `"_id" : ObjectId("5bc834a4d068620b030c5642")` dengan data baru
sebagai berikut :
{% highlight json %}
"number" : 15,
"text" : "Ahasoca Hotel"
{% endhighlight %}

Setelah itu buat query update sebagai berikut :
{% highlight mongodb %}
db.collection.update(
   {"personalDetail.address._id" : "_id" : ObjectId("5bc834a4d068620b030c5642")},
   {$set : {"personalDetail.address.$" : {
                "number" : 15,
                "text" : "Ahasoca Hotel"
            }
        }
    }
)
{% endhighlight %}

Setelah query dieksekusi, seharusnya data akan terlihat seperti ini :
{% highlight json %}
"personalDetail" : {
    "name" : "krisnanto",
    "address" : [
        {
            "_id" : ObjectId("5bc834a4d068620b030c5642"),
            "number" : 15,
            "text" : "Ahasoca Hotel"
        },
        {
            "_id" : ObjectId("5bc834a4d068620b030c5642"),
            "number" : 12,
            "text" : "Village Hotel Changi"
        }
    ]
},
{% endhighlight %}




