---
layout: home
title: "Louis Nathan Essomba"
---

<!-- ============================================================
     PERSONAL INTRODUCTION HERO
     ============================================================ -->
<section class="intro-hero">

  <div class="intro-center">
    <img src="{{ '/assets/images/me/portrait.jpg' | relative_url }}"
         alt="Portrait of Louis Nathan Essomba"
         class="intro-portrait"
         loading="lazy">

    <h1 class="intro-title">Louis Nathan Essomba</h1>
    <p class="intro-subtitle">“Building intelligence that respects humans and the Earth.”</p>

    <p class="intro-text">
      I am a young scientist‑technologist exploring the frontier between devices, intelligence, and ethics.
      This blog is my living laboratory — a place where I document my research, my projects, and the philosophy
      behind my <strong>Firmware AI thesis</strong>.  
      Here, you’ll find structured knowledge, transparent experiments, and reflections on how technology can
      remain sustainable, local, and human‑centered.
    </p>
  </div>

</section>

---

<!-- ============================================================
     FOUNDATIONS
     ============================================================ -->
<section class="section-feed">

  <h2 class="section-title">Foundations</h2>
  <p class="section-summary">
    The core ideas behind Firmware AI — thesis, vision, and the conceptual architecture that guides all my work.
  </p>

  {% assign foundations_posts = site["foundations"] | sort: "date" | reverse %}
  {% assign latest = foundations_posts | first %}

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

  {% assign most_viewed = site["foundations"] | where: "slug", "firmware-ai-cloud-library" | first %}
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

  <a href="{{ '/foundations/' | relative_url }}" class="section-link">Visit Foundations →</a>

</section>

---

<!-- ============================================================
     APPLIED WORKS
     ============================================================ -->
<section class="section-feed">

  <h2 class="section-title">Applied Works</h2>
  <p class="section-summary">
    Real‑world experiments that bring Firmware AI to life — mobile intelligence, offline SaaS, and sustainable computing.
  </p>

  {% assign applied_posts = site["applied-works"] | sort: "date" | reverse %}
  {% assign latest = applied_posts | first %}

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

  {% assign most_viewed = site["applied-works"] | where: "slug", "local-mini-ai-intro" | first %}
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

  <a href="{{ '/applied-works/' | relative_url }}" class="section-link">Visit Applied Works →</a>

</section>

---

<!-- ============================================================
     EXPLORING FRONTIERS
     ============================================================ -->
<section class="section-feed">

  <h2 class="section-title">Exploring Frontiers</h2>
  <p class="section-summary">
    Independent research exploring energy‑aware ML, AI strategies, and the future of sustainable intelligence.
  </p>

  {% assign frontier_posts = site["exploring-frontiers"] | sort: "date" | reverse %}
  {% assign latest = frontier_posts | first %}

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

  {% assign most_viewed = site["exploring-frontiers"] | where: "slug", "energy-aware-ml" | first %}
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

  <a href="{{ '/exploring-frontiers/' | relative_url }}" class="section-link">Visit Exploring Frontiers →</a>

</section>

---

<!-- ============================================================
     ETHICS & ECOLOGY
     ============================================================ -->
<section class="section-feed">

  <h2 class="section-title">Ethics & Ecology</h2>
  <p class="section-summary">
    Reflections on responsibility, sustainability, and the moral foundations of technological progress.
  </p>

  {% assign ethics_posts = site["ethics-and-ecology"] | sort: "date" | reverse %}
  {% assign latest = ethics_posts | first %}

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

  <a href="{{ '/ethics-and-ecology/' | relative_url }}" class="section-link">Visit Ethics & Ecology →</a>

</section>

---

<!-- ============================================================
     EVERYDAY INSIGHTS
     ============================================================ -->
<section class="section-feed">

  <h2 class="section-title">Everyday Insights</h2>
  <p class="section-summary">
    Notes on learning, productivity, and the daily practice of becoming a better scientist.
  </p>

  {% assign insights_posts = site["everyday-insights"] | sort: "date" | reverse %}
  {% assign latest = insights_posts | first %}

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

  {% assign most_viewed = site["everyday-insights"] | where: "slug", "studying-deep-math" | first %}
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

  <a href="{{ '/everyday-insights/' | relative_url }}" class="section-link">Visit Everyday Insights →</a>

</section>

---

<!-- ============================================================
     ABOUT ME
     ============================================================ -->
<section class="section-feed">

  <h2 class="section-title">About Me</h2>
  <p class="section-summary">
    My background, my mission, and the philosophy guiding my work.
  </p>

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
      <a href="{{ latest.url | relative_url }}" class="read-more">Read latest →</a>
    </div>
  </div>
  {% endif %}

  <a href="{{ '/about-me/' | relative_url }}" class="section-link">Visit About Me →</a>

</section>
