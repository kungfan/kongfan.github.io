---
layout: post
date: 2014-05-06
location: Hunag Gang
---

Not like wordpress or any other CMS, jekyll won't be automatically generated 
RSS feed for your blog, but there is still a simple solution for resolving  this problem .
just creat a new file named rss.xml in your directory *(in the same directory
with _config.yml)* , and paste the code below into it:

{% highlight xml %}
---
layout: nil
---
<?xml version="1.0" encoding="UTF-8"?>
<rss version="2.0" xmlns:atom="http://www.w3.org/2005/Atom">
  <channel>
    <atom:link href="http://www.paperplanes.de/rss.xml" 
    rel="self" type="application/rss+xml" />
    <title>kongfan's blog</title>
    <link>kongfan.github.io</link>
    <language>en</language>
    <webMaster>kongfan@outlook.com (KongFan)</webMaster>
    <pubDate>{{site.time | date_to_rfc822}}</pubDate>
    <copyright>Copyright 2014</copyright>
    <ttl>60</ttl>
    <description>RSS feed for KongFan's blog</description>
    {% raw %}

    {% for post in site.posts %}
    <item>
      <title>{{ post.title }}</title>
      <link>{{post.url}}</link>
      <pubDate>{{ post.date | date_to_rfc822 }}</pubDate>
      <guid>{{ post.url }}</guid>
      <description>{{ post.content | xml_escape }}</description>
    </item>
    {% endfor %}

    {% endraw %}
  </channel>
</rss>
{% endhighlight xml %}

That’s it. Jekyll will keep this file updated whenever you publish new posts
and clients will know about them .
