---
layout: page
title: Portfolio
permalink: /portfolio/
---

{% assign items = site.portfolio | sort: 'date' %}
{% for portfolio in site.portfolio reversed %}
<article class="post">
    <a class="shadow-link mod-portfolio" href="{{ site.baseurl }}{{ portfolio.url }}">
        <img class="portfolio-callout" src="{{ portfolio.callout-image }}">
        <div class="portfolio-content-small">
            <h2>{{ portfolio.title }}</h2>
            <p>{{ portfolio.excerpt }}</p>
        </div>
    </a>
</article>
{% endfor %}

