---
layout: section
title: "Independently Search"
subtitle: "Deep Scientific Exploration"
permalink: /exploring-frontiers/independently-search/
---

<!-- ============================================================
     SECTION HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">

   <img src="{{ '/assets/images/me/thinking.jpg' | relative_url }}"
         alt="Louis Nathan Essomba thinking deeply"
         class="section-portrait"
         loading="lazy">

  <h1 class="section-title-hero">Independently Search</h1>
    <p class="section-subtitle-hero">
      “To understand intelligence, one must first understand the universe it emerges from.”
    </p>
    <p class="section-description">
      Independently Search is my personal research laboratory — a space where I explore the
      scientific and philosophical foundations that shape the Firmware AI thesis.  
      This division is structured into five sub‑subsections: <strong>Mathematics</strong>,
      <strong>Physics</strong>, <strong>Chemistry</strong>, <strong>Computer Science</strong>,
      and <strong>Philosophy</strong>.  
      Each represents a frontier of knowledge, a discipline that reveals something essential
      about intelligence, structure, energy, or meaning.
    </p>

  </div>

</section>

---

<!-- ============================================================
     SUBSUBSECTION 1 — MATHEMATICS
     ============================================================ -->
<section class="subsection-feed">

  <h2 class="subsection-title">Mathematics</h2>
  <p class="subsection-summary">
    The language of structure, abstraction, and universal laws — the backbone of all reasoning.
  </p>

  <a href="{{ '/exploring-frontiers/independently-search/mathematics/' | relative_url }}"
     class="subsection-link">Visit Mathematics →</a>

  {% assign math_posts = site["exploring-frontiers"] | where: "subsubsection", "mathematics" %}
  {% assign sorted_math = math_posts | sort: "date" | reverse %}

  <!-- Latest Post -->
  {% assign latest = sorted_math | first %}
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

  <!-- Most Viewed -->
  {% assign most_viewed = math_posts | where: "slug", "math-example" | first %}
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
     SUBSUBSECTION 2 — PHYSICS
     ============================================================ -->
<section class="subsection-feed">

  <h2 class="subsection-title">Physics</h2>
  <p class="subsection-summary">
    The study of energy, matter, and the fundamental laws that govern the universe.
  </p>

  <a href="{{ '/exploring-frontiers/independently-search/physics/' | relative_url }}"
     class="subsection-link">Visit Physics →</a>

  {% assign phys_posts = site["exploring-frontiers"] | where: "subsubsection", "physics" %}
  {% assign sorted_phys = phys_posts | sort: "date" | reverse %}

  {% assign latest = sorted_phys | first %}
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

  {% assign most_viewed = phys_posts | where: "slug", "physics-example" | first %}
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
     SUBSUBSECTION 3 — CHEMISTRY
     ============================================================ -->
<section class="subsection-feed">

  <h2 class="subsection-title">Chemistry</h2>
  <p class="subsection-summary">
    The science of transformation — reactions, structures, and the emergence of complexity.
  </p>

  <a href="{{ '/exploring-frontiers/independently-search/chemistry/' | relative_url }}"
     class="subsection-link">Visit Chemistry →</a>

  {% assign chem_posts = site["exploring-frontiers"] | where: "subsubsection", "chemistry" %}
  {% assign sorted_chem = chem_posts | sort: "date" | reverse %}

  {% assign latest = sorted_chem | first %}
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

  {% assign most_viewed = chem_posts | where: "slug", "chemistry-example" | first %}
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
     SUBSUBSECTION 4 — COMPUTER SCIENCE
     ============================================================ -->
<section class="subsection-feed">

  <h2 class="subsection-title">Computer Science</h2>
  <p class="subsection-summary">
    Algorithms, computation, and the architectures that make intelligence possible.
  </p>

  <a href="{{ '/exploring-frontiers/independently-search/computer-science/' | relative_url }}"
     class="subsection-link">Visit Computer Science →</a>

  {% assign cs_posts = site["exploring-frontiers"] | where: "subsubsection", "computer-science" %}
  {% assign sorted_cs = cs_posts | sort: "date" | reverse %}

  {% assign latest = sorted_cs | first %}
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

</section>

---

<!-- ============================================================
     SUBSUBSECTION 5 — PHILOSOPHY
     ============================================================ -->
<section class="subsection-feed">

  <h2 class="subsection-title">Philosophy</h2>
  <p class="subsection-summary">
    Meaning, ethics, logic, and the foundations of thought — the soul of intelligence.
  </p>

  <a href="{{ '/exploring-frontiers/independently-search/philosophy/' | relative_url }}"
     class="subsection-link">Visit Philosophy →</a>

  {% assign philo_posts = site["exploring-frontiers"] | where: "subsubsection", "philosophy" %}
  {% assign sorted_philo = philo_posts | sort: "date" | reverse %}

  {% assign latest = sorted_philo | first %}
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

  {% assign most_viewed = philo_posts | where: "slug", "philosophy-example" | first %}
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
