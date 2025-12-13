---
layout: section
title: "About Me"
subtitle: "Identity, Mission & Journey"
permalink: /about-me/
---

<!-- ============================================================
     SECTION HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">

   <img src="{{ '/assets/images/me/formal.jpg' | relative_url }}"
         alt="Formal portrait of Louis Nathan Essomba"
         class="section-portrait"
         loading="lazy">

  <h1 class="section-title-hero">About Me</h1>

   <p class="section-subtitle-hero">
      “A mind shaped by curiosity, guided by purpose.”
    </p>

  <p class="section-description">
      My name is <strong>Louis Nathan Essomba</strong>.  
      I am a young scientist‑technologist exploring the frontier between devices, intelligence,
      ethics, and ecology.  
      This blog is the living expression of my journey — a place where I document my research,
      my experiments, my reflections, and the philosophy behind the <strong>Firmware AI thesis</strong>.
      I believe that intelligence should be sustainable, local, transparent, and deeply human.
      Everything I build, write, or explore is guided by this conviction.
    </p>

  </div>

</section>

---

<!-- ============================================================
     FEED — LATEST PERSONAL UPDATE
     ============================================================ -->
<section class="section-feed">

  <h2 class="feed-title">Latest Personal Update</h2>

  {% assign about_posts = site["about-me"] | sort: "date" | reverse %}
  {% assign latest = about_posts | first %}

  {% if latest %}
  <div class="feed-card">
    {% if latest.thumbnail %}
      <img src="{{ latest.thumbnail | relative_url }}" class="feed-thumb">
    {% endif %}
    <div class="feed-content">
      <h3>{{ latest.title }}</h3>
      <p>{{ latest.resume }}</p>
      <a href="{{ latest.url | relative_url }}" class="read-more">Read update →</a>
    </div>
  </div>
  {% endif %}

  <a href="{{ '/about-me/' | relative_url }}" class="section-link">Browse all About Me →</a>

</section>
