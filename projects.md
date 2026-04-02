---
layout: page
title: Projects
permalink: /projects/
---

<h1>Projects</h1>
<p>Here are some of the projects I’ve built — all full-stack applications with real-world impact.</p>

<div class="projects-grid">
  {% for project in site.projects %}
    <div class="project-card fade-in">

      <!-- Project content -->
      <div class="project-content">
        <h3>{{ project.title }}</h3>
        <p>{{ project.description | default: project.content | strip_html | truncate: 150 }}</p>

        {% if project.tech %}
          <ul class="project-tags">
            {% for tech in project.tech %}
              <li>{{ tech }}</li>
            {% endfor %}
          </ul>
        {% endif %}
      </div>

      <!-- Project action buttons -->
      <div class="project-footer">
        {% if project.demo %}
          <a href="{{ project.demo }}" class="button small" target="_blank">Live Demo</a>
        {% endif %}
        {% if project.github %}
          <a href="{{ project.github }}" class="button small secondary" target="_blank">GitHub</a>
        {% endif %}
      </div>

    </div>
  {% endfor %}
</div>
