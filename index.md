---
layout: page
title: Welcome!
tagline: Supporting tagline
---
{% include JB/setup %}



Thanks for visiting my website. Find more in the [about](vijayshankarv.github.io/about.html) page or read some of my articles below. 

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



