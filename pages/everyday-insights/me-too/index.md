---
layout: section
title: "Me Too"
subtitle: "Reflections Beyond the Framework"
permalink: /everyday-insights/me-too/
---

<!-- ============================================================
     HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">
    <img src="{{ '/assets/images/me/reflective.jpg' | relative_url }}"
         alt="Louis Nathan Essomba reflecting on life and news"
         class="section-portrait"
         loading="lazy">
    <h1 class="section-title-hero">Me Too</h1>
    <p class="section-subtitle-hero">
      “Thoughts that escape the system — but reveal the human behind it.”
    </p>
    <p class="section-description">
      Me Too is my free zone — the place where I write outside my core fields of science,
      engineering, and philosophy.  
      Here, I share personal reflections, reactions to news, opinions on society, and thoughts
      that don’t fit neatly into the structure of my research.  
      This subsection is spontaneous, honest, and human.  
      It captures the moments where I step back from the work and simply express myself.
    </p>

  </div>

</section>

---

<!-- ============================================================
     FEED — LATEST + MOST VIEWED
     ============================================================ -->
<section class="section-feed">

  <h2 class="feed-title">Latest Reflections</h2>

  {% assign metoo_posts = site["everyday-insights"] | where: "subsection", "me-too" | sort: "date" | reverse %}
  {% assign latest = metoo_posts | first %}

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
  {% assign most_viewed = metoo_posts | where: "slug", "opinion-example" | first %}
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

  <a href="{{ '/everyday-insights/me-too/' | relative_url }}" class="section-link">
    Browse all Me Too posts →
  </a>

</section>
