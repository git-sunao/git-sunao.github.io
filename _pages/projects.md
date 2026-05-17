---
layout: archive
title: Projects
permalink: /projects/
author_profile: true
mathjax: true
classes: justify-text

header:
  overlay_image: /assets/images/rainbow-bridge.jpg
  og_image: /assets/images/rainbow-bridge.jpg
  caption: "[Rainbow Bridge in Tokyo](https://goo.gl/maps/YZtipFQDmD1PDMpW7)"
---

My latest publication list is available at [ADS](https://ui.adsabs.harvard.edu/search/p_=0&q=pubdate%3A%5B2001-01%20TO%209999-12%5D%20(%20%20%20%3Dauthor%3A%22Sugiyama%2C%20Sunao%22%20%20%20OR%20%20%20(%3Dauthor%3A%22Sugiyama%2C%20S%22%20AND%20%3Dauthor%3A%22Jain%2C%20B%22)%20)&sort=date%20desc%2C%20bibcode%20desc).


| project | plot | description |
| ------- | ---- | ----------- |
{% for project in site.data.projectlist -%}
| [{{ project.title }}]({{ project.url | relative_url }}) | {% if project.image %}<img src="{{ project.image | relative_url }}" alt="{{ project.image_alt }}" class="project-table-img">{% endif %} | {{ project.description }} |
{% endfor %}
