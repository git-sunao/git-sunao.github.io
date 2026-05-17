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

My latest publication list is available at [ADS](<https://ui.adsabs.harvard.edu/search/filter_author_facet_hier_fq_author=AND&filter_author_facet_hier_fq_author=author_facet_hier%3A%221%2FSugiyama%2C%20S%2FSugiyama%2C%20Sunao%22&fq=%7B!type%3Daqp%20v%3D%24fq_author%7D&fq_author=(author_facet_hier%3A%221%2FSugiyama%2C%20S%2FSugiyama%2C%20Sunao%22)&q=pubdate%3A%5B2001-01%20TO%209999-12%5D%20author%3A(%22Sugiyama%2CSunao%22)&sort=date%20desc%2C%20bibcode%20desc&p_=0>).

| project | plot | description |
| ------- | ---- | ----------- |
{% for project in site.data.projectlist -%}
| [{{ project.title }}]({{ project.url | relative_url }}) | {% if project.image %}<img src="{{ project.image | relative_url }}" alt="{{ project.image_alt }}" class="project-table-img">{% endif %} | {{ project.description }} |
{% endfor %}