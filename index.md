
---
layout: default
title: "Firmware AI — Responsible Innovation"
subtitle: "A living lab notebook by Louis Nathan Essomba"
permalink: /
---

<!-- ========================= -->
<!-- HERO SECTION -->
<!-- ========================= -->

<div class="hero">
  <div class="hero-left">
    <img src="{{ '/assets/images/me/portrait.jpg' | relative_url }}" alt="Portrait of Louis Nathan Essomba" class="hero-portrait" loading="lazy">
  </div>

  <div class="hero-right">
    <h1>Welcome — I’m Louis Nathan Essomba</h1>
    <p>
      I’m a young scientist-technologist exploring the intersection of 
      <strong>AI, ethics, ecology, and device intelligence</strong>.  
      This blog is my <strong>living lab notebook</strong> — a place where I build, test, and document the 
      <strong>Firmware AI thesis</strong>.
    </p>
<div class="hero-video">
      <video controls width="100%" aria-label="Welcome message from Louis Nathan Essomba" poster="{{ '/assets/images/me/portrait.jpg' | relative_url }}">
        <source src="{{ '/assets/videos/personal/welcome-message.mp4' | relative_url }}" type="video/mp4">
        <!-- <track kind="captions" srclang="en" label="English" src="{{ '/assets/videos/personal/welcome-message.vtt' | relative_url }}"> -->
        Your browser does not support the video tag.
      </video>
    </div>
  </div>
</div>

---

# 🌌 My Vision — Firmware AI

<div class="vision-diagram">
  <img src="{{ '/assets/images/diagrams/device-cloud-firmware-ai.png' | relative_url }}" 
       alt="Diagram of Firmware AI: device ↔ cloud as algorithm library" loading="lazy">
</div>

> **Intelligence should live on devices.  
> The cloud should be a library of algorithms, not a master.**

I believe in a future where:

- Devices carry **local intelligence**  
- The cloud becomes a **temporary algorithm library**  
- Technology respects **humans** and **Earth**  
- Innovation is **ethical, ecological, and equitable**  
- Access to algorithms is **democratized**, not centralized  

This blog is where I build that future, one essay and one project at a time.

---

# 🧭 Explore the Divisions  
Each card includes a short description, a link to the section, and the **latest** + **most viewed** posts.

---

# 📚 Foundations  
### Thesis & conceptual frameworks  
[Visit section →]({{ '/foundations/' | relative_url }})

{% assign f_posts = site["foundations"] | sort: "date" | reverse %}
{% if f_posts and f_posts.size > 0 %}
  {% assign f_latest = f_posts | first %}
  {% assign f_most = site["foundations"] | sort: "views" | reverse | first %}
  **Latest:**  
  - [{{ f_latest.title }}]({{ f_latest.url | relative_url }})

  **Most viewed:**  
  {% if f_most %}
  - [{{ f_most.title }}]({{ f_most.url | relative_url }})
  {% else %}
  - [{{ f_latest.title }}]({{ f_latest.url | relative_url }})
  {% endif %}
{% else %}
  **Latest:**  
  - (No posts yet)

  **Most viewed:**  
  - (No posts yet)
{% endif %}

---

# 🛠 Applied Works  
### Real-world projects applying the thesis  
[Visit section →]({{ '/applied-works/' | relative_url }})

{% assign a_posts = site["applied-works"] | sort: "date" | reverse %}
{% if a_posts and a_posts.size > 0 %}
  {% assign a_latest = a_posts | first %}
  {% assign a_most = site["applied-works"] | sort: "views" | reverse | first %}

  **Latest:**  
  - [{{ a_latest.title }}]({{ a_latest.url | relative_url }})

  **Most viewed:**  
  {% if a_most %}
  - [{{ a_most.title }}]({{ a_most.url | relative_url }})
  {% else %}
  - [{{ a_latest.title }}]({{ a_latest.url | relative_url }})
  {% endif %}
{% else %}
  **Latest:**  
  - (No projects yet)

  **Most viewed:**  
  - (No projects yet)
{% endif %}

---

# 🌌 Exploring Frontiers  
### Independent research & company vision threads  
[Visit section →]({{ '/exploring-frontiers/' | relative_url }})

{% assign e_posts = site["exploring-frontiers"] | sort: "date" | reverse %}
{% if e_posts and e_posts.size > 0 %}
  {% assign e_latest = e_posts | first %}
  {% assign e_most = site["exploring-frontiers"] | sort: "views" | reverse | first %}

  **Latest:**  
  - [{{ e_latest.title }}]({{ e_latest.url | relative_url }})

  **Most viewed:**  
  {% if e_most %}
  - [{{ e_most.title }}]({{ e_most.url | relative_url }})
  {% else %}
  - [{{ e_latest.title }}]({{ e_latest.url | relative_url }})
  {% endif %}
{% else %}
  **Latest:**  
  - (No posts yet)

  **Most viewed:**  
  - (No posts yet)
{% endif %}

---

# 🌱 Ethics & Ecology  
### Responsibility at the core  
[Visit section →]({{ '/ethics-and-ecology/' | relative_url }})

{% assign ee_posts = site["ethics-and-ecology"] | sort: "date" | reverse %}
{% if ee_posts and ee_posts.size > 0 %}
  {% assign ee_latest = ee_posts | first %}
  {% assign ee_most = site["ethics-and-ecology"] | sort: "views" | reverse | first %}

  **Latest:**  
  - [{{ ee_latest.title }}]({{ ee_latest.url | relative_url }})

  **Most viewed:**  
  {% if ee_most %}
  - [{{ ee_most.title }}]({{ ee_most.url | relative_url }})
  {% else %}
  - [{{ ee_latest.title }}]({{ ee_latest.url | relative_url }})
  {% endif %}
{% else %}
  **Latest:**  
  - (No posts yet)

  **Most viewed:**  
  - (No posts yet)
{% endif %}

---

# 🎓 Everyday Insights  
### Student life tips & reflections on news  
[Visit section →]({{ '/everyday-insights/' | relative_url }})

{% assign i_posts = site["everyday-insights"] | sort: "date" | reverse %}
{% if i_posts and i_posts.size > 0 %}
  {% assign i_latest = i_posts | first %}
  {% assign i_most = site["everyday-insights"] | sort: "views" | reverse | first %}

  **Latest:**  
  - [{{ i_latest.title }}]({{ i_latest.url | relative_url }})

  **Most viewed:**  
  {% if i_most %}
  - [{{ i_most.title }}]({{ i_most.url | relative_url }})
  {% else %}
  - [{{ i_latest.title }}]({{ i_latest.url | relative_url }})
  {% endif %}
{% else %}
  **Latest:**  
  - (No posts yet)

  **Most viewed:**  
  - (No posts yet)
{% endif %}

---

# 👤 About Me  
### Vision, background, and how to connect  
[Visit section →]({{ '/about-me/' | relative_url }})

{% assign me_posts = site["about-me"] | sort: "date" | reverse %}
{% if me_posts and me_posts.size > 0 %}
  {% assign me_latest = me_posts | first %}
  {% assign me_most = site["about-me"] | sort: "views" | reverse | first %}

  **Latest:**  
  - [{{ me_latest.title }}]({{ me_latest.url | relative_url }})

  **Most viewed:**  
  {% if me_most %}
  - [{{ me_most.title }}]({{ me_most.url | relative_url }})
  {% else %}
  - [{{ me_latest.title }}]({{ me_latest.url | relative_url }})
  {% endif %}
{% else %}
  **Latest:**  
  - (No posts yet)

  **Most viewed:**  
  - (No posts yet)
{% endif %}

---
```
