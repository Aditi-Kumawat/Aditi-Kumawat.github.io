---
layout: page
title: Projects
permalink: /projects/
description: A curated selection of innovative projects I've contributed to over the years
nav: true
nav_order: 3
horizontal: false
---

<!-- Custom CSS for additional spacing -->
<style>
  .projects {
    margin-top: 60px; /* Adjust the value to increase or decrease the spacing */
  }
</style>

<!-- pages/projects.md -->
<div class="projects">
  <!-- Display projects without categories -->
  {% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->
  {% if page.horizontal %}
    <div class="container">
      <div class="row row-cols-1 row-cols-md-2">
      {% for project in sorted_projects %}
        {% include projects_horizontal.liquid %}
      {% endfor %}
      </div>
    </div>
  {% else %}
    <div class="row row-cols-1 row-cols-md-3">
      {% for project in sorted_projects %}
        {% include projects.liquid %}
      {% endfor %}
    </div>
  {% endif %}
</div>
