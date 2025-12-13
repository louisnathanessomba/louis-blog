---
title: "Foundations"
subtitle: "Thesis & Conceptual Frameworks"
layout: section
permalink: /foundations/
---

# Foundations — The Core of Firmware AI

The Foundations section gathers the **theoretical backbone** of the entire blog.  
Here you’ll find the **Firmware AI thesis**, conceptual frameworks, and the vision that guides all applied projects and research explorations.

Below is a curated feed of all essays in this section.  
Each card includes a visual asset, a short resume, and a link to the full form.

---

{% assign items = site.foundations | sort: "date" | reverse %}

<div class="feed">
  {% for post in items %}
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
          Read full essay →
        </a>
      </div>
</div>
  {% endfor %}
</div>
