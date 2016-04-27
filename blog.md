---
layout: page
title: Blog
permalink: /blog/
order: 3
---
<ul>
  {% for post in site.categories.blog %}
    <li>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>