---
layout: section
title: "Chemistry"
subtitle: "Transformation, Structure & Emergence"
permalink: /exploring-frontiers/independently-search/chemistry/
---

<!-- ============================================================
     HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">
    <img src="{{ '/assets/images/me/thinking.jpg' | relative_url }}"
         alt="Louis Nathan Essomba reflecting on chemistry"
         class="section-portrait"
         loading="lazy">
    <h1 class="section-title-hero">Chemistry</h1>
    <p class="section-subtitle-hero">
      “Life begins when matter learns to transform.”
    </p>
    <p class="section-description">
      Chemistry is the science of change — the study of how matter transforms, interacts,
      and organizes itself into increasingly complex structures.  
      In this subsection, I explore the molecular principles that shape everything from
      materials to biological systems.  
      These ideas help me understand emergence, energy flow, and the physical constraints
      behind sustainable computation — essential insights for the
      <strong>Firmware AI thesis</strong>.
    </p>

  </div>

</section>

---

<!-- ============================================================
     FEED — LATEST + MOST VIEWED
     ============================================================ -->
<section class="section-feed">

  <h2 class="feed-title">Latest Chemistry Explorations</h2>

  {% assign chem_posts = site["exploring-frontiers"] | where: "subsubsection", "chemistry" | sort: "date" | reverse %}
  {% assign latest = chem_posts | first %}

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
  {% assign most_viewed = chem_posts | where: "slug", "chemistry-example" | first %}
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

  <a href="{{ '/exploring-frontiers/independently-search/chemistry/' | relative_url }}"
     class="section-link">Browse all Chemistry →</a>

</section>
