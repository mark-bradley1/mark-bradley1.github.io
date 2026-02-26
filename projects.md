---
layout: page
title: Projects
permalink: /projects/
---

# Projects

{% raw %}
{% for project in site.projects %}
<div class="card">
  <h3>
    <a href="{{ project.url }}">{{ project.title }}</a>
  </h3>
  <p>{{ project.content | strip_html | truncate: 120 }}</p>
  <small>{{ project.tech }}</small>
</div>
{% endfor %}
{% endraw %}
