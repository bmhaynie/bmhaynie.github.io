---
layout: page
title: Beer
permalink: /beer/
order: 1
---

<ul class="post-list">
	{% assign sorted_beer = site.categories.beer | sort: 'title' %}
		{% for post in sorted_beer %}
		  <li>
		    <h2>
		      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
			      {{ post.title }} ({{ post.beer-style }})
					<!-- <img src="{{ site.baseurl }}/images/{{ post.image }}"> -->
		      </a>

		    </h2>
		  </li>
		{% endfor %}
</ul>