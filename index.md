---
layout: page
title: noSQL, yesSQL & Couchbase
tagline: a distributed cache, kv & document database with SQL
---
{% include JB/setup %}

## About me

{% highlight json %}
{
  "firstname": "terry",
  "lastname": "dhariwal",
  "employer": "Couchbase",
  "role": "noSQL Architect & Developer",
  "email": [
             "terry@couchbase.com",
             "terry.dhariwal@me.com"
           ]
}
{% endhighlight %}

## About this blog

This is my personal blog about noSQL and [Couchbase](http://www.couchbase.com) - a open source swiss-army-knife noSQL database. It's a:

* distributed HA Caching
* distributed HA Key Value database
* distributed HA Document database
* with ANSI compliant and extended SQL for document queries
 

This blog <del>contains</del> will provide a series of articles to get you started with noSQL and Couchbase. 

It <del>also explores</del> will also explore specific use-cases and advanced topics that are all too often not documented.  

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

