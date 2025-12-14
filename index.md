---
layout: home
title: "Louis Nathan Essomba"
---

<!-- ============================================================
     HERO (already rewritten earlier)
     ============================================================ -->
<section class="hero">
  <div class="hero-inner">

    <img src="{{ '/assets/images/me/portrait.jpg' | relative_url }}"
         alt="Portrait of Louis Nathan Essomba"
         class="hero-portrait"
         loading="lazy">

    <div class="hero-text">
      <h1 class="hero-title">Louis Nathan Essomba</h1>
      <p class="hero-tagline">Building intelligence that respects humans and the Earth.</p>
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
     SECTION FEEDS (using feed-block.html)
     ============================================================ -->

{% include feed-block.html
   title="Foundations"
   posts=site.foundations
   most_viewed="firmware-ai-cloud-library"
   link="/foundations/"
   link_text="Visit Foundations →"
%}

{% include feed-block.html
   title="Applied Works"
   posts=site["applied-works"]
   most_viewed="local-mini-ai-intro"
   link="/applied-works/"
   link_text="Visit Applied Works →"
%}

{% include feed-block.html
   title="Exploring Frontiers"
   posts=site["exploring-frontiers"]
   most_viewed="energy-aware-ml"
   link="/exploring-frontiers/"
   link_text="Visit Exploring Frontiers →"
%}

{% include feed-block.html
   title="Ethics & Ecology"
   posts=site["ethics-and-ecology"]
   most_viewed="ethics-ecology-interdependence"
   link="/ethics-and-ecology/"
   link_text="Visit Ethics & Ecology →"
%}

{% include feed-block.html
   title="Everyday Insights"
   posts=site["everyday-insights"]
   most_viewed="studying-deep-math"
   link="/everyday-insights/"
   link_text="Visit Everyday Insights →"
%}

{% include feed-block.html
   title="About Me"
   posts=site["about-me"]
   link="/about-me/"
   link_text="Visit About Me →"
%}
