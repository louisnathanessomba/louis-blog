---
title: "Foundations"
subtitle: "Thesis & Conceptual Frameworks"
layout: default
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
      <img src="{{ post.thumbnail }}" alt="{{ post.title }} thumbnail" class="thumb">
      <div class="content">
        <h2>{{ post.title }}</h2>
        <p>{{ post.resume }}</p>
        <a class="read-more" href="{{ site.baseurl }}{{ post.url }}">
          Read full essay →
        </a>
      </div>
    </div>
  {% endfor %}
</div>
    
