---
layout: single
title: "Virtualization Notes"
permalink: /notes/category/virtualization/
author_profile: true
---

{% assign sorted_notes = site.notes | where_exp: "item", "item.category downcase == 'virtualization'" | sort: "date" | reverse %}

<p>Found {{ sorted_notes | size }} notes in category 'virtualization'.</p>

{% for note in sorted_notes %}
  {% include archive-single.html %}
{% endfor %}
