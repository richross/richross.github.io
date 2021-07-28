---
permalink: /index.html
layout: default
title: Home Page
author: 
  twitter: rich_ross
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>