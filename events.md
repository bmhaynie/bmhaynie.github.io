---
layout: page
title: Events
permalink: /events/
order: 2
---
<ul>
  {% for post in site.categories.event %}
    <li>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>