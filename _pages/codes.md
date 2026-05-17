---
layout: archive
title: Codes
permalink: /codes/
author_profile: true
mathjax: true
classes: justify-text

header:
  overlay_image: /assets/images/camp-dinner.jpg
  og_image: /assets/images/camp-dinner.jpg
  caption: "Dinner in camp during cycling tour."
---

| name | website | internal page | description |
| ---- | ------- | ------------- | ----------- |
{% for code in site.data.codelist -%}
| {{ code.name }} | [{{ code.website_name }}]({{ code.website_url }}) | [{{ code.internal_name }}]({{ code.internal_url | relative_url }}) | {{ code.description }} |
{% endfor %}