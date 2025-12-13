---
layout: section
title: "Exploring Frontiers"
subtitle: "Research & Comparative Analysis"
permalink: /exploring-frontiers/
---

<!-- ============================================================
     SECTION HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">

<img src="{{ '/assets/images/me/thinking.jpg' | relative_url }}"
         alt="Louis Nathan Essomba thinking"
         class="section-portrait"
         loading="lazy">

<h1 class="section-title-hero">Exploring Frontiers</h1>

<p class="section-subtitle-hero">
      “Where curiosity meets the unknown, and ideas become discoveries.”
    </p>

<p class="section-description">
      Exploring Frontiers is my research space — a place where I dive into the scientific,
      philosophical, and technological foundations that enrich the Firmware AI thesis.
      This division is split into two complementary paths: <strong>Independently Search</strong>,
      where I explore core disciplines such as mathematics, physics, chemistry, computer science,
      and philosophy; and <strong>Companies Threads</strong>, where I analyze and compare the visions
      of major technology companies shaping the future of intelligence.
    </p>

  </div>

</section>

---

<!-- ============================================================
     SUBSECTION 1 — INDEPENDENTLY SEARCH
     ============================================================ -->
<section class="subsection-feed">

  <h2 class="subsection-title">Independently Search</h2>
  <p class="subsection-summary">
    Deep dives into scientific and philosophical disciplines — the raw material that fuels
    the Firmware AI paradigm.
  </p>

  <a href="{{ '/exploring-frontiers/independently-search/' | relative_url }}"
     class="subsection-link">Visit Independently Search →</a>

  {% assign indep_posts = site["exploring-frontiers"] | where: "subsection", "independently-search" %}
  {% assign sorted_indep = indep_posts | sort: "date" | reverse %}

  <!-- Latest Post -->
  {% assign latest = sorted_indep | first %}
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
  {% assign most_viewed = indep_posts | where: "slug", "energy-aware-ml" | first %}
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

</section>

---

<!-- ============================================================
     SUBSECTION 2 — COMPANIES THREADS
     ============================================================ -->
<section class="subsection-feed">

  <h2 class="subsection-title">Companies Threads</h2>
  <p class="subsection-summary">
    Comparative analyses of major technology companies — their strategies, architectures,
    philosophies, and how they align or diverge from the Firmware AI vision.
  </p>

  <a href="{{ '/exploring-frontiers/companies-threads/' | relative_url }}"
     class="subsection-link">Visit Companies Threads →</a>

  {% assign company_posts = site["exploring-frontiers"] | where: "subsection", "companies-threads" %}
  {% assign sorted_company = company_posts | sort: "date" | reverse %}

  <!-- Latest Post -->
  {% assign latest = sorted_company | first %}
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
  {% assign most_viewed = company_posts | where: "slug", "microsoft-vs-google" | first %}
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

</section>
