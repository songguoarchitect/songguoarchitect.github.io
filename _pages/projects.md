---
layout: page
title: Projects
permalink: /projects/
description: Research projects and grants I participate as the main contributor
nav: true
nav_order: 5
display_categories: [ongoing, completed]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">

{%- comment -%}
安全地获取 projects 集合：
优先从 site.collections 里拿 label=projects 的 docs；否则回退到 site.projects；
若仍然为 nil，则设为空数组，避免 sort on nil。
{%- endcomment -%}
{% assign projects_collection = site.collections | where: "label", "projects" | first %}
{% if projects_collection %}
  {% assign all_projects = projects_collection.docs %}
{% else %}
  {% assign all_projects = site.projects | default: empty %}
{% endif %}

{%- comment -%} 过滤未发布 {%- endcomment -%}
{% assign all_projects = all_projects | where_exp: "p", "p.published != false" %}

{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
    <a id="{{ category }}" href=".#{{ category }}">
      <h2 class="category">{{ category }}</h2>
    </a>

    {%- comment -%} 分类后兜底为空数组 {%- endcomment -%}
    {% assign categorized_projects = all_projects | where: "category", category | default: empty %}

    {%- comment -%} 只有有内容时才排序，避免对空/未定义排序 {%- endcomment -%}
    {% if categorized_projects and categorized_projects.size > 0 %}
      {% assign sorted_projects = categorized_projects | sort: "importance" %}
    {% else %}
      {% assign sorted_projects = empty %}
    {% endif %}

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

    {% if sorted_projects.size == 0 %}
      <p>No projects in category <code>{{ category }}</code> yet.</p>
    {% endif %}

  {% endfor %}

{% else %}

  <!-- Display projects without categories -->
  {% if all_projects and all_projects.size > 0 %}
    {% assign sorted_projects = all_projects | sort: "importance" %}
  {% else %}
    {% assign sorted_projects = empty %}
  {% endif %}

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

  {% if sorted_projects.size == 0 %}
    <p>No projects yet. Add items to <code>/_projects/</code> to populate this page.</p>
  {% endif %}

{% endif %}
</div>
