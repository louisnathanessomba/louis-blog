---
layout: section
title: "Computer Science"
subtitle: "Computation, Architecture & Intelligent Systems"
permalink: /exploring-frontiers/independently-search/computer-science/
---

<!-- ============================================================
     HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">
    <img src="{{ '/assets/images/me/thinking.jpg' | relative_url }}"
         alt="Louis Nathan Essomba thinking about computation"
         class="section-portrait"
         loading="lazy">
    <h1 class="section-title-hero">Computer Science</h1>
    <p class="section-subtitle-hero">
      “Intelligence is not magic — it is architecture.”
    </p>
    <p class="section-description">
      Computer Science is the study of computation, algorithms, and the architectures that make
      intelligent systems possible.  
      In this subsection, I explore the principles behind software design, data structures,
      distributed systems, complexity, and the foundations of modern AI.  
      These explorations directly feed into the <strong>Firmware AI thesis</strong>, helping me
      understand how to build systems that are efficient, local, sustainable, and aligned with
      human needs.
    </p>

  </div>

</section>

---

<!-- ============================================================
     FEED — LATEST + MOST VIEWED
     ============================================================ -->
<section class="section-feed">

  <h2 class="feed-title">Latest Computer Science Explorations</h2>

  {% assign cs_posts = site["exploring-frontiers"] | where: "subsubsection", "computer-science" | sort: "date" | reverse %}
  {% assign latest = cs_posts | first %}

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
  {% assign most_viewed = cs_posts | where: "slug", "cs-example" | first %}
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

  <a href="{{ '/exploring-frontiers/independently-search/computer-science/' | relative_url }}"
     class="section-link">Browse all Computer Science →</a>

</section>
