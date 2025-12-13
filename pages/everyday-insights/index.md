---
layout: section
title: "Everyday Insights"
subtitle: "Life, Learning & Perspective"
permalink: /everyday-insights/
---

<!-- ============================================================
     SECTION HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">

<img src="{{ '/assets/images/me/studying.jpg' | relative_url }}"
         alt="Louis Nathan Essomba studying and reflecting"
         class="section-portrait"
         loading="lazy">
    <h1 class="section-title-hero">Everyday Insights</h1>
    <p class="section-subtitle-hero">
      “Growth happens in the quiet moments — the ones no one sees.”
    </p>
    <p class="section-description">
      Everyday Insights is the human side of my journey — the space where I share what I learn
      outside of formal research and engineering.  
      This division is divided into two subsections: <strong>Student Life Tips</strong>, where I
      document my methods, struggles, and strategies as a student in the scientific department;
      and <strong>Me Too</strong>, a more personal zone where I reflect on news, society, and
      the world beyond my core fields.  
      These insights are small, honest, and grounded — the everyday fuel behind my larger work.
    </p>

  </div>

</section>

---

<!-- ============================================================
     SUBSECTION 1 — STUDENT LIFE TIPS
     ============================================================ -->
<section class="subsection-feed">

  <h2 class="subsection-title">Student Life Tips</h2>
  <p class="subsection-summary">
    Practical strategies, study methods, and reflections from my daily life as a student.
  </p>

  <a href="{{ '/everyday-insights/student-life-tips/' | relative_url }}"
     class="subsection-link">Visit Student Life Tips →</a>

  {% assign slt_posts = site["everyday-insights"] | where: "subsection", "student-life-tips" %}
  {% assign sorted_slt = slt_posts | sort: "date" | reverse %}

  <!-- Latest Post -->
  {% assign latest = sorted_slt | first %}
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
  {% assign most_viewed = slt_posts | where: "slug", "study-methods-example" | first %}
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
     SUBSECTION 2 — ME TOO
     ============================================================ -->
<section class="subsection-feed">

  <h2 class="subsection-title">Me Too</h2>
  <p class="subsection-summary">
    Personal reflections, opinions on news, and thoughts that live outside my main fields.
  </p>

  <a href="{{ '/everyday-insights/me-too/' | relative_url }}"
     class="subsection-link">Visit Me Too →</a>

  {% assign metoo_posts = site["everyday-insights"] | where: "subsection", "me-too" %}
  {% assign sorted_metoo = metoo_posts | sort: "date" | reverse %}

  <!-- Latest Post -->
  {% assign latest = sorted_metoo | first %}
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

</section>
