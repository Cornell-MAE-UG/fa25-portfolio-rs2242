---
layout: default
title: Projects
permalink: /projects/
---

<div class="gallery-container">
  <div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
        <a class="project-link" href="{{ project.url | relative_url }}">
          <div class="project-card">
            <div class="project-title">{{ project.title }}</div>
            {% if project.description %}
              <div class="project-desc">{{ project.description }}</div>
            {% endif %}
          </div>
        </a>
      </div>
    {% endfor %}
  </div>
</div>
