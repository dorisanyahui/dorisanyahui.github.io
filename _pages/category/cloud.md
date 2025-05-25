---
layout: archive
title: "Cloud Notes"
permalink: /notes/category/cloud/
author_profile: true
category: cloud
---

{% include base_path %}

{% assign sorted_notes = site.notes | where: "category", page.category | sort: "date" | reverse %}
{% for note in sorted_notes %}
  {% include archive-single.html %}
{% endfor %}
