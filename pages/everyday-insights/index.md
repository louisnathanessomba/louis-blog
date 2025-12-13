---
layout: section
title: "Everyday Insights"
subtitle: "Student life tips and commentary on news"
permalink: /everyday-insights/
---

# Everyday Insights — Life & Reflections

Everyday Insights is the most personal division of the blog.  
It gathers reflections from my student life, practical strategies for productivity and balance, and commentary on news or events that resonate with my vision of responsible innovation.

Below, you’ll find two curated feeds:
- **Student Life Tips** → practical advice, study methods, productivity, balance  
- **Me Too** → opinions and reflections on news and societal issues  

Each post includes a visual asset, a short resume, and a link to the full form.

---

# 🎓 Student Life Tips  
### Practical strategies from my journey as a scientific student

{% assign tips_posts = site["everyday-insights"] 
     | where_exp: "item", "item.categories contains 'student-life-tips'" 
     | sort: "date" 
     | reverse %}

<div class="feed">
  {% for post in tips_posts %}
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

# 📰 Me Too  
### Opinions and reflections on news and events

{% assign me_too_posts = site["everyday-insights"] 
     | where_exp: "item", "item.categories contains 'me-too'" 
     | sort: "date" 
     | reverse %}

<div class="feed">
  {% for post in me_too_posts %}
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
          Read full reflection →
        </a>
      </div>
    </div>
  {% endfor %}
</div>
