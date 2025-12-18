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
          <p><strong>{{ project.title }}</strong></p>
          {% if project.description %}
            <p>{{ project.description }}</p>
          {% endif %}
        </a>
      </div>
    {% endfor %}
  </div>
</div>

