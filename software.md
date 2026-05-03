---
layout: page
title: Software
permalink: /software/
---

# Software

This section collects software projects, numerical tools, and reproducible
research codes.

{% for project in site.software %}
<div class="card">
  <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
  <p>{{ project.summary }}</p>

  {% if project.github %}
  <p><a href="{{ project.github }}">GitHub repository</a></p>
  {% endif %}
</div>
{% endfor %}
