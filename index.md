---
layout: page
title: About James Tang
tagline: 
---

{% include JB/setup %}

An iOS Application Developer practices to think as a Designer

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



