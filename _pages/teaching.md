---
layout: page
permalink: /courses/
title: Teachings
description: Teaching materials
nav: true
nav_order: 4
---

<!-- <ul>
<li>[<a href="/teaching/2024-fall-cv">CIS 4930/CIS 5930: Computer Vision</a>]</li>
</ul> -->

<!-- pages/projects.md -->
<div class="courses">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.courses | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
</div>