---
layout: archive
title: "Virtualization Notes"
permalink: /notes/category/virtualization/
author_profile: true
---

{% include base_path %}

{% assign sorted_notes = site.notes | where: "category", "virtualization" | sort: "date" | reverse %}

{% for note in sorted_notes %}
  {% include archive-single.html %}
{% endfor %}
