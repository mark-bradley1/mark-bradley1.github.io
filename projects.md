---
layout: page
permalink: /projects/
---

<h1>Projects</h1>
<p>Here are some of the projects I’ve built — all full-stack applications with real-world impact.</p>

<div class="projects-grid">
  {% for project in site.projects %}
    <div class="card project-card">

      <div class="project-header">
        <h3>{{ project.title }}</h3>
        {% if project.type %}
          <span class="badge">{{ project.type }}</span>
        {% endif %}
      </div>

      <p class="project-description">
        {{ project.description }}
      </p>

      <div class="project-tech">
        {% for tech in project.stack %}
          <span>{{ tech }}</span>
        {% endfor %}
      </div>

      <div class="project-links">
        {% if project.demo %}
          <a href="{{ project.demo }}" class="button small">Live Demo</a>
        {% endif %}
        {% if project.github %}
          <a href="{{ project.github }}" target="_blank">GitHub →</a>
        {% endif %}
      </div>

    </div>
  {% endfor %}
</div>
