---
layout: archive
title: "Virtualization Notes"
permalink: /notes/category/virtualization/
author_profile: true
category: virtualization
---

{% include base_path %}

{% assign sorted_notes = site.notes | where: "category", page.category | sort: "date" | reverse %}
{% for note in sorted_notes %}
  {% include archive-single.html %}
{% endfor %}
