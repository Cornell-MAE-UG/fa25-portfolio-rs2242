---
layout: default
title: Projects
permalink: /projects/
---

<div style="max-width: 900px; margin: 40px auto; padding: 0 20px;">
  <h1 style="margin-bottom: 10px;">Projects</h1>
  <div style="opacity:0.8; margin-bottom: 20px;">
    Projects found: {{ site.projects | size }}
  </div>

  {% for project in site.projects %}
    <div style="border:1px solid rgba(0,0,0,0.18); border-radius:12px; padding:16px; margin-bottom:14px; background:#fff;">
      <a href="{{ project.url | relative_url }}" style="text-decoration:none; color:#111 !important; display:block;">
        <div style="font-weight:700; font-size:18px; line-height:1.3; margin-bottom:6px; color:#111 !important;">
          {{ project.title }}
        </div>

        {% if project.description %}
          <div style="opacity:0.85; line-height:1.4; color:#111 !important;">
            {{ project.description }}
          </div>
        {% endif %}
      </a>
    </div>
  {% endfor %}
</div>
