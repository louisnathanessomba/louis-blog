---
layout: home
title: "Louis Nathan Essomba"
---

<!-- ============================================================
     HERO — CLEAN, MINIMAL, PROFESSIONAL
     ============================================================ -->
<section class="hero">
  <div class="hero-inner">
    <img src="{{ '/assets/images/me/portrait.jpg' | relative_url }}"
         alt="Portrait of Louis Nathan Essomba"
         class="hero-portrait"
         loading="lazy">
    <div class="hero-text">
      <h1 class="hero-title">Louis Nathan Essomba</h1>
      <p class="hero-tagline">
        Building intelligence that respects humans and the Earth.
      </p>
      <p class="hero-description">
        I am a young scientist‑technologist exploring the frontier between devices,
        intelligence, and ethics.  
        This blog is my living laboratory — a place where I document my research,
        my projects, and the philosophy behind my <strong>Firmware AI thesis</strong>.
      </p>
    </div>

  </div>
</section>

---

<!-- ============================================================
     SECTION FEED TEMPLATE (REUSED)
     ============================================================ -->

{% include section-feed.html
   title="Foundations"
   summary="The core ideas behind Firmware AI — thesis, vision, and conceptual architecture."
   collection="foundations"
   most_viewed_slug="firmware-ai-cloud-library"
   section_url="/foundations/"
%}

{% include section-feed.html
   title="Applied Works"
   summary="Real‑world experiments that bring Firmware AI to life — mobile intelligence, offline SaaS, and sustainable computing."
   collection="applied-works"
   most_viewed_slug="local-mini-ai-intro"
   section_url="/applied-works/"
%}

{% include section-feed.html
   title="Exploring Frontiers"
   summary="Independent research exploring energy‑aware ML, AI strategies, and the future of sustainable intelligence."
   collection="exploring-frontiers"
   most_viewed_slug="energy-aware-ml"
   section_url="/exploring-frontiers/"
%}

{% include section-feed.html
   title="Ethics & Ecology"
   summary="Reflections on responsibility, sustainability, and the moral foundations of technological progress."
   collection="ethics-and-ecology"
   most_viewed_slug="ethics-ecology-interdependence"
   section_url="/ethics-and-ecology/"
%}

{% include section-feed.html
   title="Everyday Insights"
   summary="Notes on learning, productivity, and the daily practice of becoming a better scientist."
   collection="everyday-insights"
   most_viewed_slug="studying-deep-math"
   section_url="/everyday-insights/"
%}

{% include section-feed.html
   title="About Me"
   summary="My background, my mission, and the philosophy guiding my work."
   collection="about-me"
   section_url="/about-me/"
%}
