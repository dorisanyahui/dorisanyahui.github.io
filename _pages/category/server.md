---
layout: archive
title: "Server Notes"
permalink: /notes/category/server/
author_profile: true
category: server
---

{% include base_path %}

{% assign sorted_notes = site.notes | where: "category", page.category | sort: "date" | reverse %}
{% for note in sorted_notes %}
  {% include archive-single.html %}
{% endfor %}
