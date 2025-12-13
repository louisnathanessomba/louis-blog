---
layout: section
title: "About Me"
subtitle: "Vision, background, and how to connect"
permalink: /about-me/
---

# About Me — Louis Nathan Essomba

I am a young scientist-technologist in the scientific department of Première, with strong foundations in mathematics, physics, chemistry, and computer science.  
Beyond school programs, I pursue advanced research independently, building projects that serve as proofs of concept for my **Firmware AI thesis** — a vision for sustainable, local, ethical intelligence.

This page introduces my vision, skills, philosophy, and ongoing projects.  
At the end, you’ll find a dynamic feed of personal posts and updates.

---

# 🌌 Vision

My long-term mission is to democratize access to algorithms and reduce dependence on centralized elites.  
Through **Firmware AI**, I envision devices with local intelligence, borrowing models from the cloud as a temporary algorithm library — always guided by ethics and ecology.

---

# 🛠 Skills & Interests

- Informatics, coding (Markdown, HTML, CSS, JS, system architecture)  
- Advanced reasoning in mathematics, physics, chemistry  
- Project management and technical documentation  
- Responsible innovation in AI, Big Data, and cloud computing  
- Ethics and ecology integrated into every project  

---

# 📚 Current Projects

### 📱 Local Mini AI Project  
A mobile app testing local intelligence through conditional and iterative structures.  
It explores probability, statistics, and machine learning at the device level.  
**Explore →**  
[Visit project]({{ '/applied-works/local-mini-ai/' | relative_url }})

### 🌍 Offline-First SaaS for the South  
A sustainable platform for digitalization in underserved regions, built on Raspberry Pi.  
It applies Firmware AI to reduce cloud dependency and improve digital resilience.  
**Explore →**  
[Visit project]({{ '/applied-works/offline-first-saas/' | relative_url }})

---

# 🌱 Philosophy

Technology must respect its maker — **humans** — and the environment — **Earth**.  
Every project I build is designed with responsibility, sustainability, and equity at its core.  
Ethics and ecology are not optional add-ons; they are the **firmware of innovation**.

---

# 📝 Personal Feed  
### Updates, reflections, and personal notes

{% assign about_posts = site["about-me"] | sort: "date" | reverse %}

<div class="feed">
  {% for post in about_posts %}
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

# 📬 Contact

- **Email:** louisnathanessomba@gmail.com  
- **GitHub:** https://github.com/louisnathanessomba  
- **Blog Home:** [Home]({{ '/' | relative_url }})

Feel free to reach out for collaboration, discussion, or mentorship.
