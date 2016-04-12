---
layout: page
title: Beer
permalink: /beer/
order: 1
---

<ul>
	{% for beer in site.beer %}
		<li><a href="{{ beer.url | prepend: site.baseurl }}">{{ beer.title }}</a></li>
	{% endfor %}
</ul>