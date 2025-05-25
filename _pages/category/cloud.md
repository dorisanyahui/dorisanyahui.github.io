---
layout: archive
title: "Cloud Notes"
permalink: /notes/category/cloud/
author_profile: true
---

{% include base_path %}

{% assign category_name = page.url | split: '/' | last | downcase %}
{% assign notes_in_category = site.notes | where: "category", category_name %}
{% assign sorted_notes = notes_in_category | sort: "date" | reverse %}

{% for note in sorted_notes %}
  <div class="archive__item">
    <h3 class="archive__item-title">
      <a href="{{ note.url | relative_url }}">{{ note.title }}</a>
    </h3>
    <p><small>{{ note.date | date: "%B %d, %Y" }}</small></p>
    {% if note.excerpt %}
      <p>{{ note.excerpt | strip_html | truncate: 150 }}</p>
    {% else %}
      <p>{{ note.content | strip_html | truncate: 150 }}</p>
    {% endif %}
  </div>
  <hr />
{% endfor %}
