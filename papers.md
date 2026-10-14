---
layout: page
title: Papers
description: "Papers and related notes."
permalink: /papers/
---

{% assign papers = site.papers | sort_natural: 'title' %}
<ul>
{% for paper in papers %}
  <li>
    <a href="{{ paper.url | relative_url }}">{{ paper.title | escape }}</a>
    {% if paper.description %}<p>{{ paper.description | escape }}</p>{% endif %}
  </li>
{% endfor %}
</ul>
{% if papers.size == 0 %}<p>No papers listed yet.</p>{% endif %}
