---
layout: archive
title: "Research Projects"
permalink: /research/
author_profile: false
---

{% include base_path %}

{% for post in site.research reversed %}
  {% include archive-single.html %}
{% endfor %}
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}