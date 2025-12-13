---
layout: home
title: "Firmware AI — Responsible Innovation"
subtitle: "A living lab notebook by Louis Nathan Essomba"
permalink: /
---

<!-- ========================= -->
<!-- HYBRID HERO (handled by layout: home) -->
<!-- ========================= -->

<!-- The hero is rendered automatically by default.html when layout == "home" -->


<!-- ========================= -->
<!-- VISION SECTION -->
<!-- ========================= -->

# 🌌 My Vision — Firmware AI

<div class="vision-diagram">
  <img src="{{ '/assets/images/diagrams/device-cloud-firmware-ai.png' | relative_url }}"
       alt="Firmware AI conceptual diagram"
       loading="lazy">
</div>

> **Intelligence should live on devices.  
> The cloud should be a library of algorithms, not a master.**

I believe in a future where:

- Devices carry **local intelligence**  
- The cloud becomes a **temporary algorithm library**  
- Technology respects **humans** and **Earth**  
- Innovation is **ethical, ecological, and equitable**  
- Access to algorithms is **democratized**, not centralized  


---

# 🧭 Explore the Divisions

Below are the six divisions of this blog.  
Each section includes **latest** and **most viewed** posts.

---

## Foundations  
### Thesis & conceptual frameworks  
[Visit section →]({{ '/foundations/' | relative_url }})

{% assign f_posts = site.foundations | sort: "date" | reverse %}
{% if f_posts.size > 0 %}
  {% assign f_latest = f_posts | first %}
  **Latest:**  
  - [{{ f_latest.title }}]({{ f_latest.url | relative_url }})

  {% assign f_most = site.foundations | sort: "views" | reverse | first %}
  **Most viewed:**  
  - [{{ f_most.title }}]({{ f_most.url | relative_url }})
{% else %}
  _No posts yet._
{% endif %}

---

## Applied Works  
### Real-world projects applying the thesis  
[Visit section →]({{ '/applied-works/' | relative_url }})

{% assign a_posts = site["applied-works"] | sort: "date" | reverse %}
{% if a_posts.size > 0 %}
  {% assign a_latest = a_posts | first %}
  **Latest:**  
  - [{{ a_latest.title }}]({{ a_latest.url | relative_url }})

  {% assign a_most = site["applied-works"] | sort: "views" | reverse | first %}
  **Most viewed:**  
  - [{{ a_most.title }}]({{ a_most.url | relative_url }})
{% else %}
  _No posts yet._
{% endif %}

---

## Exploring Frontiers  
### Independent research & company vision threads  
[Visit section →]({{ '/exploring-frontiers/' | relative_url }})

{% assign e_posts = site["exploring-frontiers"] | sort: "date" | reverse %}
{% if e_posts.size > 0 %}
  {% assign e_latest = e_posts | first %}
  **Latest:**  
  - [{{ e_latest.title }}]({{ e_latest.url | relative_url }})

  {% assign e_most = site["exploring-frontiers"] | sort: "views" | reverse | first %}
  **Most viewed:**  
  - [{{ e_most.title }}]({{ e_most.url | relative_url }})
{% else %}
  _No posts yet._
{% endif %}

---

## Ethics & Ecology  
### Responsibility at the core  
[Visit section →]({{ '/ethics-and-ecology/' | relative_url }})

{% assign ee_posts = site["ethics-and-ecology"] | sort: "date" | reverse %}
{% if ee_posts.size > 0 %}
  {% assign ee_latest = ee_posts | first %}
  **Latest:**  
  - [{{ ee_latest.title }}]({{ ee_latest.url | relative_url }})

  {% assign ee_most = site["ethics-and-ecology"] | sort: "views" | reverse | first %}
  **Most viewed:**  
  - [{{ ee_most.title }}]({{ ee_most.url | relative_url }})
{% else %}
  _No posts yet._
{% endif %}

---

## Everyday Insights  
### Student life tips & reflections  
[Visit section →]({{ '/everyday-insights/' | relative_url }})

{% assign i_posts = site["everyday-insights"] | sort: "date" | reverse %}
{% if i_posts.size > 0 %}
  {% assign i_latest = i_posts | first %}
  **Latest:**  
  - [{{ i_latest.title }}]({{ i_latest.url | relative_url }})

  {% assign i_most = site["everyday-insights"] | sort: "views" | reverse | first %}
  **Most viewed:**  
  - [{{ i_most.title }}]({{ i_most.url | relative_url }})
{% else %}
  _No posts yet._
{% endif %}

---

## About Me  
### Vision, background, and how to connect  
[Visit section →]({{ '/about-me/' | relative_url }})

{% assign me_posts = site["about-me"] | sort: "date" | reverse %}
{% if me_posts.size > 0 %}
  {% assign me_latest = me_posts | first %}
  **Latest:**  
  - [{{ me_latest.title }}]({{ me_latest.url | relative_url }})

  {% assign me_most = site["about-me"] | sort: "views" | reverse | first %}
  **Most viewed:**  
  - [{{ me_most.title }}]({{ me_most.url | relative_url }})
{% else %}
  _No posts yet._
{% endif %}

