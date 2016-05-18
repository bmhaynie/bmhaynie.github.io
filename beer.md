---
layout: base
title: All Beer
permalink: /beer/
---

<section id="beer" class="page bg-light-gray">
    <div class="container">
        <div class="row text-center">
            <div class="col-xs-12">
                <h2 class="section-heading">{{ page.title }}</h2>
            </div>
        </div>
        <div class="row">
            {% for beer in site.beer %}
                <div class="col-lg-3 col-md-4 col-sm-6 col-xs-12 beer-item">
                    <a href="{{ beer.url }}" class="beer-link">
                        <div class="beer-hover">
                            <div class="beer-hover-content">
                                <i class="fa fa-search-plus fa-3x"></i>
                            </div>
                        </div>
                        <img src="/img/beer/{{ beer.img }}" class="img-responsive img-centered" alt="">
                    </a>
                    <div class="beer-caption">
                        <h3>{{ beer.title }}</h3>
                        <p class="text-muted">{{ beer.style }}</p>
                        <p><span>{{ beer.abv }}</span></p>
                    </div>
                </div>
            {% endfor %}
        </div>
    </div>
</section>