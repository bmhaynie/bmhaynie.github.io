---
layout: page
title: Beer
permalink: /beer/
order: 1
---

Lorem ipsum dolor sit amet, consectetur adipiscing elit. 

<ul class="post-list">
	{% for post in site.categories.beer %}
	  <li>
	    <h2>
	      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
		      {{ post.title }}<br>
					<img src="{{ site.baseurl }}/images/{{ post.image }}">
	      </a>

	    </h2>
	  </li>
	{% endfor %}
</ul>