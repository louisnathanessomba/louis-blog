---
layout: section
title: "Student Life Tips"
subtitle: "Learning, Discipline & Daily Growth"
permalink: /everyday-insights/student-life-tips/
---

<!-- ============================================================
     HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">
    <img src="{{ '/assets/images/me/studying.jpg' | relative_url }}"
         alt="Louis Nathan Essomba studying"
         class="section-portrait"
         loading="lazy">
    <h1 class="section-title-hero">Student Life Tips</h1>
    <p class="section-subtitle-hero">
      “Mastery is built one quiet hour at a time.”
    </p>
    <p class="section-description">
      Student Life Tips is where I share the strategies, habits, and reflections that guide my
      daily life as a student in the scientific department.  
      These notes are practical and honest — from study methods and time management to motivation,
      discipline, and the mental frameworks that help me grow.  
      This subsection is the human engine behind my larger work: the routines that make the
      impossible possible.
    </p>

  </div>

</section>

---

<!-- ============================================================
     FEED — LATEST + MOST VIEWED
     ============================================================ -->
<section class="section-feed">

  <h2 class="feed-title">Latest Tips & Notes</h2>

  {% assign slt_posts = site["everyday-insights"] | where: "subsection", "student-life-tips" | sort: "date" | reverse %}
  {% assign latest = slt_posts | first %}

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

  <a href="{{ '/everyday-insights/student-life-tips/' | relative_url }}" class="section-link">
    Browse all Student Life Tips →
  </a>

</section>
