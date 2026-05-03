---
layout: page
title: Research & Publications
permalink: /research-publications/
---

# Research & Publications

My research lies at the interface of theoretical astrophysics, astroparticle
physics, gravitational-wave physics, and computational modeling.

I study compact objects as extreme laboratories for dark matter and
beyond-standard-model physics. In particular, I am interested in how neutron
stars, binary neutron-star systems, strong magnetic fields, dense matter, and
dynamical spacetime curvature can generate observable signatures of hidden
sectors.

My research trajectory has evolved from boson stars and gravastar models to
dark-matter effects in neutron stars, gravitational-wave signatures in compact
binaries, and axion/ALP–photon couplings in strongly magnetized relativistic
systems.

## Research lines

{% for item in site.research %}
<div class="card">
  <h3><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h3>
  <p>{{ item.summary }}</p>
</div>
{% endfor %}

## Selected publications

<div class="card publication">
  <h3>Probing ALP-photon couplings in Neutron Stars: scalar versus pseudoscalar cases</h3>
  <p>D. Suárez-Fontanella, C. Albertus, M. Pérez-García</p>
  <p><strong>Physical Review D</strong>, 2025</p>
  <p>
    <a href="https://doi.org/10.1103/gv6n-89k2">View publication</a>
  </p>
</div>

<div class="card publication">
  <h3>Gravitational Wave emission in Binary Neutron Star early post-merger within a dark environment</h3>
  <p>D. Suárez-Fontanella, D. Barba-González, C. Albertus, M. Pérez-García</p>
  <p><strong>Physics Letters B</strong>, 2025</p>
  <p>
    <a href="https://doi.org/10.1016/j.physletb.2025.139358">View publication</a>
  </p>
</div>

<div class="card publication">
  <h3>The Science of the Einstein Telescope</h3>
  <p>Einstein Telescope Collaboration, including D. Suárez-Fontanella</p>
  <p><strong>Journal of Cosmology and Astroparticle Physics</strong>, 2026</p>
  <p>
    Contributor to Section 7: Subatomic Physics with ET.
  </p>
  <p>
    <a href="https://doi.org/10.1088/1475-7516/2026/03/081">View publication</a>
  </p>
</div>

## Full publication list

{% for paper in site.data.publications %}
<div class="card publication">
  <h3>{{ paper.title }}</h3>
  <p>{{ paper.authors }}</p>

  <p>
    <strong>{{ paper.venue }}</strong>{% if paper.year %}, {{ paper.year }}{% endif %}
  </p>

  {% if paper.note %}
  <p>{{ paper.note }}</p>
  {% endif %}

  {% if paper.arxiv %}
  <p>arXiv: {{ paper.arxiv }}</p>
  {% endif %}

  {% if paper.doi %}
  <p>DOI: <a href="{{ paper.doi }}">{{ paper.doi }}</a></p>
  {% endif %}

  {% if paper.url %}
  <p><a href="{{ paper.url }}">View publication</a></p>
  {% endif %}
</div>
{% endfor %}

## External profiles

- [ORCID](https://orcid.org/0000-0002-3891-0187)
- [INSPIRE-HEP](https://inspirehep.net/authors/2914623)
- [GitHub](https://github.com/Du92)