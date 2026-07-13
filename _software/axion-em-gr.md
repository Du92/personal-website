---
layout: page
title: axion_em_gr
summary: "Python package for exploratory axion-Maxwell simulations on fixed 3+1 backgrounds."
github: "https://github.com/Du92/aXemg"
---

# axion_em_gr

`axion_em_gr` is a Python package for exploratory numerical studies of
axion-Maxwell dynamics on fixed 3+1 backgrounds.

The package is designed around a modular architecture for grids, field states,
background geometries, physical sources, diagnostics, evolution schemes, and
post-processing. Its goal is to provide a flexible research tool for testing
reduced models of axion electrodynamics in relativistic astrophysical
environments.

## Main features

- Modular Python architecture.
- Fixed-background 3+1 geometries.
- Axion and electromagnetic field evolution.
- Diagnostic tools for constraints and field invariants.
- YAML-based configuration and reproducible runs.
- Plotting and post-processing utilities for scientific visualization.

## Example simulation

The video below shows an example exploratory simulation produced with
`axion_em_gr`, illustrating the evolution of axion-electromagnetic fields in a
fixed 3+1 background.

<figure class="video-figure">
  <video controls muted playsinline preload="metadata"
         poster="{{ '/assets/images/research/axion-em-gr-gw-halo-poster.png' | relative_url }}">
    <source src="{{ '/assets/videos/research/axion_em_summary.mp4' | relative_url }}"
            type="video/mp4">
    Your browser does not support the video tag.
  </video>

  <figcaption>
    Example simulation of axion-electromagnetic dynamics generated with
    <code>axion_em_gr</code>. The animation illustrates the qualitative response
    of the axion and electromagnetic fields in a fixed relativistic background.
  </figcaption>
</figure>

{% for project in site.software %}
<div class="card">
  <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
  <p>{{ project.summary }}</p>

  {% if project.github %}
  <p><a href="{{ project.github }}">GitHub repository</a></p>
  {% endif %}
</div>
{% endfor %}