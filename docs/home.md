---
permalink: /home.html
author: 
  twitter: rich_ross
---


## This is just the home page.

<ul>
  {% for post in site.drafts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>