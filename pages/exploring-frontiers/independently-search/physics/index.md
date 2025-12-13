---
layout: section
title: "Physics"
subtitle: "Energy, Matter & Universal Laws"
permalink: /exploring-frontiers/independently-search/physics/
---

<!-- ============================================================
     HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">
    <img src="{{ '/assets/images/me/thinking.jpg' | relative_url }}"
         alt="Louis Nathan Essomba reflecting on physics"
         class="section-portrait"
         loading="lazy">
    <h1 class="section-title-hero">Physics</h1>
    <p class="section-subtitle-hero">
      “To understand reality, follow the flow of energy.”
    </p>
    <p class="section-description">
      Physics is the study of the universe at its most fundamental level.  
      In this subsection, I explore the principles that govern motion, energy, fields, matter,
      and the deep structures that shape everything from atoms to galaxies.  
      These explorations help me understand the physical constraints and opportunities behind
      computation, devices, and sustainable intelligence — essential pillars of the
      <strong>Firmware AI thesis</strong>.
    </p>

  </div>

</section>

---

<!-- ============================================================
     FEED — LATEST + MOST VIEWED
     ============================================================ -->
<section class="section-feed">

  <h2 class="feed-title">Latest Physics Explorations</h2>

  {% assign phys_posts = site["exploring-frontiers"] | where: "subsubsection", "physics" | sort: "date" | reverse %}
  {% assign latest = phys_posts | first %}

  <!-- Latest Post -->
  {% if latest %}
  <div class="feed-card">
    {% if latest.thumbnail %}
      <img src="{{ latest.thumbnail | relative_url }}" class="feed-thumb">
    {% endif %}
    <div class="feed-content">
      <h3>{{ latest.title }}</h3>
      <p>{{ latest.resume }}</p>
      <a href="{{ latest.url | relative_url }}" class="read-more">Read latest →</a>
    </div>
  </div>
  {% endif %}

  <!-- Most Viewed (manual selection) -->
  {% assign most_viewed = phys_posts | where: "slug", "physics-example" | first %}
  {% if most_viewed %}
  <div class="feed-card">
    {% if most_viewed.thumbnail %}
      <img src="{{ most_viewed.thumbnail | relative_url }}" class="feed-thumb">
    {% endif %}
    <div class="feed-content">
      <h3>{{ most_viewed.title }}</h3>
      <p>{{ most_viewed.resume }}</p>
      <a href="{{ most_viewed.url | relative_url }}" class="read-more">Most viewed →</a>
    </div>
  </div>
  {% endif %}

  <a href="{{ '/exploring-frontiers/independently-search/physics/' | relative_url }}"
     class="section-link">Browse all Physics →</a>

</section>
