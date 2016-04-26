---
layout: page
<!-- title: Beer -->
permalink: /beer/
order: 1
---

<!-- show beer names and links -->
<ul>
	{% for beer in site.beer %}
		<li><a href="{{ beer.url | prepend: site.baseurl }}">{{ beer.title }}</a></li>
	{% endfor %}
</ul>

<!-- show beer details -->
<!-- <section>
	<ul>
		{% for beer in site.beer %}
			<li class="test">
				{{ beer.title }}
				{{ beer.beer-abv }}
				{{ beer.beer-availability }}
				{{ beer.beer-bitterness }}
				{{ beer.beer-gravity }}
				{{ beer.beer-sourness }}
				{{ beer.beer-style }}
				{{ beer.content }}
			</li>
		{% endfor %}
	</ul>
</section> -->