---
layout: page
title: Teaching
permalink: /teaching/
---

# Teaching

This section collects teaching activities, lecture notes, problem sheets, and
short educational notes for students.

My teaching experience includes undergraduate-level activities in general
relativity, quantum field theory, nuclear astrophysics, mechanics, and
oscillations laboratories. During my PhD, I have also contributed as a teaching
assistant and university lecturer at the University of Salamanca.

## Teaching experience

<div class="card">
  <h3>University of Salamanca</h3>
  <p class="meta">Teaching Assistant / University Lecturer · 2024–2025</p>
  <ul>
    <li>A Journey to Nuclear Astrophysics and its Mathematical Foundations.</li>
    <li>Mechanics and Oscillations Laboratory.</li>
  </ul>
</div>

<div class="card">
  <h3>ICIMAF</h3>
  <p class="meta">Teaching Assistant · 2020–2021</p>
  <ul>
    <li>Introduction to General Relativity.</li>
    <li>Quantum Field Theory.</li>
  </ul>
</div>

## Downloadable teaching notes

{% for note in site.data.teaching_notes %}
<div class="card">
  <h3>{{ note.title }}</h3>

  <p class="meta">
    {{ note.course }} · {{ note.level }} · {{ note.language }}
  </p>

  <p>{{ note.description }}</p>

  <p>
    <a class="button" href="{{ note.file | relative_url }}">Download PDF</a>
  </p>
</div>
{% endfor %}

## Short notes

{% for note in site.notes %}
<div class="card">
  <h3><a href="{{ note.url | relative_url }}">{{ note.title }}</a></h3>

  {% if note.date %}
  <p class="meta">{{ note.date | date: "%B %d, %Y" }}</p>
  {% endif %}

  <p>{{ note.summary }}</p>
</div>
{% endfor %}
