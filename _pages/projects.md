---
layout: default
title: Rushil Sharan - Portfolio
permalink: /projects/
---

<div style="max-width: 900px; margin: 40px auto; padding: 0 20px;">
  <h1 style="margin-bottom: 20px;">Projects</h1>

  <p style="opacity:0.8; margin-bottom: 20px;">
    Projects found: {{ site.projects | size }}
  </p>

  {% for project in site.projects %}
    <div style="border:1px solid rgba(0,0,0,0.15); border-radius:12px; padding:16px; margin-bottom:14px; background:white;">
      <a href="{{ project.url | relative_url }}" style="text-decoration:none; color:inherit;">
        <div style="font-weight:700; font-size:18px; margin-bottom:6px;">
          {{ project.title }}
        </div>

        {% if project.description %}
          <div style="opacity:0.85; margin-bottom:10px;">
            {{ project.description }}
          </div>
        {% endif %}

        {% if project.image %}
          <img src="{{ project.image | absolute_url }}" alt="{{ project.title }}"
               style="width:100%; max-width:700px; height:auto; display:block; border-radius:10px; margin-top:10px;" />
        {% endif %}
      </a>
    </div>
  {% endfor %}
</div>
