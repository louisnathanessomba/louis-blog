---
layout: section
title: "Applied Works"
subtitle: "Data-driven projects applying the thesis"
permalink: /applied-works/
---

# Applied Works — Proofs of Concept

Applied Works gathers all projects that bring the **Firmware AI thesis** into real-world contexts.  
Each project is structured into multiple posts — introduction, technical details, and ethical–ecological reflections — forming a complete, transparent documentation of the work.

Below, you’ll find a dynamic feed of all Applied Works posts, grouped by project.  
Each card includes a visual asset, a short resume, and a link to the full post.

---

# 📱 Local Mini AI Project  
### A mobile experiment in local intelligence

{% assign local_posts = site["applied-works"] 
     | where_exp: "item", "item.categories contains 'local-mini-ai'" 
     | sort: "date" 
     | reverse %}

<div class="feed">
  {% for post in local_posts %}
    <div class="card">

      {% if post.thumbnail %}
        <img src="{{ post.thumbnail | relative_url }}" 
             alt="{{ post.title }} thumbnail" 
             class="thumb" loading="lazy">
      {% endif %}

      <div class="content">
        <h2>{{ post.title }}</h2>

        {% if post.resume %}
          <p>{{ post.resume }}</p>
        {% endif %}

        <a class="read-more" href="{{ post.url | relative_url }}">
          Read full post →
        </a>
      </div>

    </div>
  {% endfor %}
</div>

---

# 🌍 Offline-First SaaS for the South  
### A sustainable platform for Africa and South America

{% assign saas_posts = site["applied-works"] 
     | where_exp: "item", "item.categories contains 'offline-first-saas'" 
     | sort: "date" 
     | reverse %}

<div class="feed">
  {% for post in saas_posts %}
    <div class="card">
 {% if post.thumbnail %}
        <img src="{{ post.thumbnail | relative_url }}" 
             alt="{{ post.title }} thumbnail" 
             class="thumb" loading="lazy">
      {% endif %}
  <div class="content">
        <h2>{{ post.title }}</h2>
 {% if post.resume %}
          <p>{{ post.resume }}</p>
        {% endif %}
<a class="read-more" href="{{ post.url | relative_url }}">
          Read full post →
        </a>
      </div>
</div>
  {% endfor %}
</div>
