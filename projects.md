---
layout: page
title: Projects
permalink: /projects/
---

<div class="projects-grid">
  {% for project in site.projects %}
    <div class="card">
      <h3>
        <a href="{{ project.url | relative_url }}">
          {{ project.title }}
        </a>
      </h3>
      <p>{{ project.content | strip_html | truncate: 120 }}</p>
      <small>{{ project.tech }}</small>
    </div>
  {% endfor %}
</div>
