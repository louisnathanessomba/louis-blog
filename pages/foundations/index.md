---
layout: section
title: "Foundations"
subtitle: "Core Ideas & Vision"
permalink: /foundations/
---

<!-- ============================================================
     SECTION HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">

  <img src="{{ '/assets/images/me/conceptual.jpg' | relative_url }}"
         alt="Louis Nathan Essomba reflecting on ideas"
         class="section-portrait"
         loading="lazy">

  <h1 class="section-title-hero">Foundations</h1>
    <p class="section-subtitle-hero">
      “Every system begins with a philosophy — every philosophy begins with a question.”
    </p>
    <p class="section-description">
      Foundations is the conceptual core of my work.  
      This is where the <strong>Firmware AI thesis</strong> is shaped, challenged, refined, and expanded.
      Here, I explore the principles that guide my entire vision: decentralization, sustainability,
      human‑centered intelligence, and the idea that technology should empower rather than dominate.
      These essays form the intellectual backbone of everything I build — the theory before the practice,
      the architecture before the code, the meaning before the mechanism.
    </p>

  </div>

</section>

---

<!-- ============================================================
     FEED — LATEST + MOST VIEWED
     ============================================================ -->
<section class="section-feed">

  <h2 class="feed-title">Core Essays</h2>

  {% assign foundation_posts = site["foundations"] | sort: "date" | reverse %}
  {% assign latest = foundation_posts | first %}

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
  {% assign most_viewed = site["foundations"] | where: "slug", "firmware-ai-thesis" | first %}
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

  <a href="{{ '/foundations/' | relative_url }}" class="section-link">Browse all Foundations →</a>

</section>
