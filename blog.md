---
layout: default
title: Blog
permalink: /blog/
---

[← Back to Home](/)

# Blog

<div style="display:flex; flex-wrap:wrap; gap:20px; justify-content:center;">

{% for post in site.posts %}
  <div style="border:1px solid #ccc; padding:15px; width:300px; box-sizing:border-box;">
    <h2 style="margin-top:0;"><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p style="font-size:0.85em; color:#666;">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.content | strip_html | truncatewords: 30 }}</p>
    <a href="{{ post.url }}">Read More →</a>
  </div>
{% endfor %}

</div>
