---
layout: section
title: "Everyday Insights"
subtitle: "Life, Learning & Perspective"
permalink: /everyday-insights/
---

<!-- HERO -->
<section class="section-hero">
  {% include hero.html
     portrait="/assets/images/me/studying.jpg"
     alt="Louis Nathan Essomba studying and reflecting"
     title=page.title
     subtitle=page.subtitle
     description="Everyday Insights is the human side of my journey — the space where I share what I learn outside of formal research and engineering. This division is divided into two subsections: Student Life Tips, where I document my methods, struggles, and strategies as a student in the scientific department; and Me Too, a more personal zone where I reflect on news, society, and the world beyond my core fields. These insights are small, honest, and grounded — the everyday fuel behind my larger work."
  %}
</section>

---

<!-- SUBSECTION 1 — STUDENT LIFE TIPS -->
<section class="subsection-feed">

  <h2 class="subsection-title">Student Life Tips</h2>
  <p class="subsection-summary">
    Practical strategies, study methods, and reflections from my daily life as a student.
  </p>

  <a href="{{ '/everyday-insights/student-life-tips/' | relative_url }}"
     class="subsection-link">Visit Student Life Tips →</a>

  {% assign slt_posts = site["everyday-insights"] | where: "subsection", "student-life-tips" %}

  {% include feed.html
     title="Latest from Student Life Tips"
     posts=slt_posts
     most_viewed="study-methods-example"
     link="/everyday-insights/student-life-tips/"
     link_text="Browse all Student Life Tips →"
  %}

</section>

---

<!-- SUBSECTION 2 — ME TOO -->
<section class="subsection-feed">

  <h2 class="subsection-title">Me Too</h2>
  <p class="subsection-summary">
    Personal reflections, opinions on news, and thoughts that live outside my main fields.
  </p>

  <a href="{{ '/everyday-insights/me-too/' | relative_url }}"
     class="subsection-link">Visit Me Too →</a>

  {% assign metoo_posts = site["everyday-insights"] | where: "subsection", "me-too" %}

  {% include feed.html
     title="Latest from Me Too"
     posts=metoo_posts
     most_viewed="opinion-example"
     link="/everyday-insights/me-too/"
     link_text="Browse all Me Too →"
  %}

</section>
