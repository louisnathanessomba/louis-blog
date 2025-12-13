---
layout: section
title: "Ethics & Ecology"
subtitle: "Responsibility & Sustainability"
permalink: /ethics-and-ecology/
---

<!-- ============================================================
     SECTION HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">

  <img src="{{ '/assets/images/me/reflective.jpg' | relative_url }}"
         alt="Louis Nathan Essomba reflecting on ethics and ecology"
         class="section-portrait"
         loading="lazy">

  <h1 class="section-title-hero">Ethics & Ecology</h1>

  <p class="section-subtitle-hero">
      “Technology is powerful — but power means nothing without responsibility.”
    </p>

  <p class="section-description">
      Ethics & Ecology is the moral compass of my work.  
      This section explores the responsibilities we carry as creators of intelligent systems:
      the ecological cost of computation, the ethical implications of automation, the balance
      between progress and preservation, and the duty to design technologies that respect both
      humanity and the planet.  
      These essays form the conscience of the Firmware AI thesis — a reminder that innovation
      must remain sustainable, transparent, and deeply human.
    </p>

  </div>

</section>

---

<!-- ============================================================
     FEED — LATEST + MOST VIEWED
     ============================================================ -->
<section class="section-feed">

  <h2 class="feed-title">Ethical & Ecological Essays</h2>

  {% assign ethics_posts = site["ethics-and-ecology"] | sort: "date" | reverse %}
  {% assign latest = ethics_posts | first %}

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
  {% assign most_viewed = site["ethics-and-ecology"] | where: "slug", "ethics-ecology-interdependence" | first %}
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

  <a href="{{ '/ethics-and-ecology/' | relative_url }}" class="section-link">Browse all Ethics & Ecology →</a>

</section>
