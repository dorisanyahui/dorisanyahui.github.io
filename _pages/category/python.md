---
layout: archive
title: "Python Notes"
permalink: /notes/category/python/
author_profile: true
category: python
---

{% include base_path %}

{% assign sorted_notes = site.notes | where: "category", page.category | sort: "date" | reverse %}
{% for note in sorted_notes %}
  {% include archive-single.html %}
{% endfor %}
