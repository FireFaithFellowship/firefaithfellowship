---
layout: default
title: Studies
---
# One‑Page Studies

<ul>
{% assign items = site.studies | sort: 'title' %}
{% for s in items %}
  <li><a href="{{ s.url | relative_url }}">{{ s.title }}</a>{% if s.subtitle %} — <em>{{ s.subtitle }}</em>{% endif %}</li>
{% endfor %}
</ul>
