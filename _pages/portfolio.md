---
layout: page
title: Portfolio
permalink: /portfolio/
---

<!-- ## [Badger Maps](/portfolio/badger-maps)
### 2013-2019
While at Badger I designed and implemented a responsive webapp, a native iOS app, and a native Android app. I also revamped the logo, helped implement a brand identity along with another designer, created plenty of collateral, and more. Here's a little sampling. -->

{% for portfolio in site.portfolio %}
  <h2>
    <a href="{{ portfolio.url }}">
      {{ portfolio.title }}
    </a>
  </h2>
{% endfor %}

{% include portfolio.html image-url="/images/badger-main-image.png" description="Design for Badger Maps" piece-title="whaaat" piece-date="2017" %}

## [Hank](/portfolio/hank)
### 2019
Branding work for Hank, an AI powered HVAC controller for commercial buildings

## [Pocket Bodhi](/portfolio/pocket-bodhi)
### 2015
Concept app design for a meditation application

## [Rocky Mountain Ruby](/portfolio/rocky-mountain-ruby)
### 2015
Branding work for a ruby conference in Denver

## [Associates Dein](/portfolio/associates-dein)
### 2013
Website and design/product work for an interactive map of the valley to show listings based on neighborhood

## [Fahrenheit Labs](/portfolio/fahrenheit-labs)
### 2009-2012
Some branding and website work for a design agency I cofounded

## [CloudHike](/portfolio/cloudhike)
### 2011
Concept branding and website for a cloud hosting company focused on wordpress

## [Owle Bubo](/portfolio/owle)
### 2009
Website design for a iPhone product that made filming much more stable