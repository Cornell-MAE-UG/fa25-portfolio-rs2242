---
layout: default
title: Rushil Sharan - Portfolio
permalink: /projects/
---

<div class="gallery-container">
  <div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
        <p>{{ project.title }}</p>
      </div>
    {% endfor %}
  </div>
</div>

