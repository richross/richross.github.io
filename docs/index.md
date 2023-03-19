---
permalink: /index.html
layout: default
author: 
  twitter: rich_ross
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a><br/>
      <b>{{ post.date | date_to_string }}</b>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>