---
layout: section
title: "Exploring Frontiers"
subtitle: "Research & Comparative Analysis"
permalink: /exploring-frontiers/
---

<!-- HERO -->
<section class="section-hero">
  {% include hero.html
     portrait="/assets/images/me/thinking.jpg"
     alt="Louis Nathan Essomba thinking"
     title=page.title
     subtitle=page.subtitle
     description="Exploring Frontiers is my research space — a place where I dive into the scientific, philosophical, and technological foundations that enrich the Firmware AI thesis. This division is split into two complementary paths: Independently Search, where I explore core disciplines such as mathematics, physics, chemistry, computer science, and philosophy; and Companies Threads, where I analyze and compare the visions of major technology companies shaping the future of intelligence."
  %}
</section>

---

<!-- SUBSECTION 1 — INDEPENDENTLY SEARCH -->
<section class="subsection-feed">

  <h2 class="subsection-title">Independently Search</h2>
  <p class="subsection-summary">
    Deep dives into scientific and philosophical disciplines — the raw material that fuels
    the Firmware AI paradigm.
  </p>

  <a href="{{ '/exploring-frontiers/independently-search/' | relative_url }}"
     class="subsection-link">Visit Independently Search →</a>

  {% assign indep_posts = site["exploring-frontiers"] | where: "subsection", "independently-search" %}

  {% include feed.html
     title="Latest from Independently Search"
     posts=indep_posts
     most_viewed="energy-aware-ml"
     link="/exploring-frontiers/independently-search/"
     link_text="Browse all Independently Search →"
  %}

</section>

---

<!-- SUBSECTION 2 — COMPANIES THREADS -->
<section class="subsection-feed">

  <h2 class="subsection-title">Companies Threads</h2>
  <p class="subsection-summary">
    Comparative analyses of major technology companies — their strategies, architectures,
    philosophies, and how they align or diverge from the Firmware AI vision.
  </p>

  <a href="{{ '/exploring-frontiers/companies-threads/' | relative_url }}"
     class="subsection-link">Visit Companies Threads →</a>

  {% assign company_posts = site["exploring-frontiers"] | where: "subsection", "companies-threads" %}

  {% include feed.html
     title="Latest from Companies Threads"
     posts=company_posts
     most_viewed="microsoft-vs-google"
     link="/exploring-frontiers/companies-threads/"
     link_text="Browse all Companies Threads →"
  %}

</section>
