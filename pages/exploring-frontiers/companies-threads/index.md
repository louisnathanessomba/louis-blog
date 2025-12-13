---
layout: section
title: "Companies Threads"
subtitle: "Visions, Strategies & Technological Philosophies"
permalink: /exploring-frontiers/companies-threads/
---

<!-- ============================================================
     HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">
    <img src="{{ '/assets/images/me/thinking.jpg' | relative_url }}"
         alt="Louis Nathan Essomba analyzing technology companies"
         class="section-portrait"
         loading="lazy">
    <h1 class="section-title-hero">Companies Threads</h1>
    <p class="section-subtitle-hero">
      “To understand the future, study those who are building it.”
    </p>
    <p class="section-description">
      Companies Threads is where I analyze the strategies, architectures, and philosophies of
      major technology companies.  
      Each thread is a deep dive into how these organizations think about intelligence,
      sustainability, data, devices, and the future of computing.  
      This subsection helps me compare their visions with the <strong>Firmware AI thesis</strong>,
      revealing alignments, divergences, and lessons that shape my own work.
    </p>

  </div>

</section>

---

<!-- ============================================================
     FEED — LATEST + MOST VIEWED
     ============================================================ -->
<section class="section-feed">

  <h2 class="feed-title">Latest Company Threads</h2>

  {% assign ct_posts = site["exploring-frontiers"] | where: "subsection", "companies-threads" | sort: "date" | reverse %}
  {% assign latest = ct_posts | first %}

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
  {% assign most_viewed = ct_posts | where: "slug", "microsoft-vs-google" | first %}
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

  <a href="{{ '/exploring-frontiers/companies-threads/' | relative_url }}" class="section-link">
    Browse all Company Threads →
  </a>

</section>
