---
layout: section
title: "Mathematics"
subtitle: "The Language of Structure"
permalink: /exploring-frontiers/independently-search/mathematics/
---

<!-- ============================================================
     HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">
    <img src="{{ '/assets/images/me/thinking.jpg' | relative_url }}"
         alt="Louis Nathan Essomba thinking about mathematics"
         class="section-portrait"
         loading="lazy">
    <h1 class="section-title-hero">Mathematics</h1>
    <p class="section-subtitle-hero">
      “Behind every phenomenon lies a structure — behind every structure, a truth.”
    </p>
    <p class="section-description">
      Mathematics is the foundation of all rigorous thought.  
      In this subsection, I explore the concepts, abstractions, and frameworks that shape
      my understanding of intelligence, computation, and the physical world.  
      From algebraic structures to analysis, from geometry to probability, mathematics is the
      silent architecture behind the Firmware AI thesis — the pure language that reveals how
      systems behave, evolve, and interact.
    </p>

  </div>

</section>

---

<!-- ============================================================
     FEED — LATEST + MOST VIEWED
     ============================================================ -->
<section class="section-feed">

  <h2 class="feed-title">Latest Mathematical Explorations</h2>

  {% assign math_posts = site["exploring-frontiers"] | where: "subsubsection", "mathematics" | sort: "date" | reverse %}
  {% assign latest = math_posts | first %}

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
  {% assign most_viewed = math_posts | where: "slug", "math-example" | first %}
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

  <a href="{{ '/exploring-frontiers/independently-search/mathematics/' | relative_url }}"
     class="section-link">Browse all Mathematics →</a>

</section>
