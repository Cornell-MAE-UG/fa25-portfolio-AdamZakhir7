---
layout: default
title: Adam Zakhir - Portfolio
permalink: /projects/
---

{% for project in site.projects %}
  {% if project.title == "Fluid-Mechanical Dissection" %}
  <div class="project-card">
    <a href="{{ project.url | relative_url }}">
      <img src="{{ project.image | relative_url }}" alt="{{ project.title }}">
      <h2>{{ project.title }}</h2>
    </a>
    <p>{{ project.description }}</p>
  </div>
  {% endif %}
{% endfor %}
