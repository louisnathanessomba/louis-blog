---
layout: section
title: "Exploring Frontiers"
subtitle: "Independent research and company vision threads"
permalink: /exploring-frontiers/
---

# Exploring Frontiers — Research & Comparative Analysis

Exploring Frontiers is the division where I push beyond the core thesis and dive into the **scientific, philosophical, and industrial landscapes** that shape the future of technology.  
It is structured into two complementary subsections:

- **Independently Search** → deep dives into mathematics, physics, chemistry, computer science, and philosophy  
- **Companies Threads** → comparative analyses of major tech companies and their visions  

Below is a curated feed of all posts from both subsections, each presented with a visual asset, a short resume, and a link to the full essay.

---

# 🔬 Independently Search  
### Deep dives into scientific and philosophical foundations

{% assign research_posts = site["exploring-frontiers"] 
     | where_exp: "item", "item.categories contains 'independently-search'" 
     | sort: "date" 
     | reverse %}

<div class="feed">
  {% for post in research_posts %}
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

---

# 🏢 Companies Threads  
### Comparative analyses of major tech visions

{% assign company_posts = site["exploring-frontiers"] 
     | where_exp: "item", "item.categories contains 'companies-threads'" 
     | sort: "date" 
     | reverse %}

<div class="feed">
  {% for post in company_posts %}
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
          Read full analysis →
        </a>
      </div>
 </div>
  {% endfor %}
</div>
