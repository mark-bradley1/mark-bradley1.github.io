<section id="projects" class="fade-in">

  <div class="section-header">
    <h2>Projects</h2>
    <a href="{{ '/projects/' | relative_url }}">View All →</a>
  </div>

  <div class="projects-grid">

    {% for project in site.projects limit:2 %}
      <div class="card project-card"
        onclick="window.location='{{ project.url | relative_url }}'">

        <div class="project-header">
          <h3>{{ project.title }}</h3>
          {% if project.type %}
            <span class="badge">{{ project.type }}</span>
          {% endif %}
        </div>

        <p class="project-description">
          {{ project.description }}
        </p>

        <ul class="project-tags">
          {% for tech in project.stack %}
            <li>{{ tech }}</li>
          {% endfor %}
        </ul>

        <div class="project-footer">
          {% if project.github and project.github != "" %}
             <a href="{{ project.github | strip }}" 
             class="button small" 
             target="_blank" 
             rel="noopener noreferrer">
             onclick="event.stopPropagation();">
              GitHub
            </a>
          {% else %}
            <span style="color:red;">Missing GitHub link</span>
          {% endif %}
        </div>
      </div>
    {% endfor %}
  </div>
</section>
