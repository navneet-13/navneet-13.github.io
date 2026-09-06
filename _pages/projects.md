---
layout: page
title: projects
permalink: /projects/
description: A growing collection of my projects in computer architecture, ML systems, hardware, and robotics.
nav: true
nav_order: 2
display_categories: [research, ml, hardware, robotics]
---

<!-- pages/projects.md -->
<div class="projects-list">
{%- if site.enable_project_categories and page.display_categories %}
  {%- for category in page.display_categories %}
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" -%}
  {%- if sorted_projects.size > 0 %}
  <h2 class="category text-capitalize">{{ category }}</h2>
  {%- for project in sorted_projects %}
  <h3 class="mt-3 mb-1"><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
  <p>{{ project.description }}</p>
  {%- endfor %}
  {%- endif %}
  {%- endfor %}
{%- else -%}
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  {%- for project in sorted_projects %}
  <h3 class="mt-3 mb-1"><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
  <p>{{ project.description }}</p>
  {%- endfor %}
{%- endif -%}
</div>
