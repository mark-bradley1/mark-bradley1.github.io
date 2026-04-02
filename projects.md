---
layout: page
title: Projects
permalink: /projects/
---

<div class="projects-grid">
  {% for project in site.projects %}
    <div class="card">
      <h3>{{ project.title }}</h3>
      <p>{{ project.description | default: project.content | strip_html | truncate: 120 }}</p>
      
      {% if project.tech %}
        <small>
          {% for t in project.tech %}
            {{ t }}{% unless forloop.last %}, {% endunless %}
          {% endfor %}
        </small>
      {% endif %}

      <div class="project-footer" style="margin-top:0.8rem;">
        {% if project.github %}
          <a href="{{ project.github }}" class="button small secondary" target="_blank">GitHub</a>
        {% endif %}
        {% if project.demo %}
          <a href="{{ project.demo }}" class="button small" target="_blank">Live Demo</a>
        {% endif %}
      </div>
    </div>
  {% endfor %}
</div>
