---
layout: default
title: Rushil Sharan - Portfolio
permalink: /projects/
---

<div class="gallery-container">
  <div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
        <a href="{{ project.url | relative_url }}">
          <div class="thumb">
            {% if project.image %}
              <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
            {% endif %}
          </div>
          <div class="meta">
            <p class="proj-title">{{ project.title }}</p>
            {% if project.description %}
              <p class="proj-desc">{{ project.description }}</p>
            {% endif %}
          </div>
        </a>
      </div>
    {% endfor %}
  </div>
</div>

