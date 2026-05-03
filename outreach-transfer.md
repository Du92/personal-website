---
layout: page
title: Outreach & Transfer
permalink: /outreach-transfer/
---

# Outreach & Transfer

This section collects outreach initiatives, personal projects, science
communication activities, and transfer-oriented work connecting physics,
data science, education, and society.

My outreach and transfer activities include science communication projects,
independent initiatives, applied data-science collaborations, and
industry-facing work where scientific methods are used beyond a purely academic
context.

## Projects

{% for project in site.outreach_transfer %}
<div class="card">
  <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>

  {% if project.category %}
  <p class="meta">{{ project.category }}{% if project.year %} · {{ project.year }}{% endif %}</p>
  {% elsif project.year %}
  <p class="meta">{{ project.year }}</p>
  {% endif %}

  <p>{{ project.summary }}</p>

  {% if project.external_url %}
  <p><a href="{{ project.external_url }}">External link</a></p>
  {% endif %}
</div>
{% endfor %}