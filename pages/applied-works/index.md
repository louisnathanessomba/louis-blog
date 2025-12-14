---
layout: section
title: "Applied Works"
subtitle: "Proofs of Concept"
permalink: /applied-works/
---

<!-- HERO -->
<section class="section-hero">
  {% include hero.html
     portrait="/assets/images/me/working.jpg"
     alt="Louis Nathan Essomba working on computer"
     title=page.title
     subtitle=page.subtitle
     description="Applied Works gathers all my real‑world experiments built from the Firmware AI thesis. Each project is a complete ecosystem: an introduction to the idea, a deep dive into the technical architecture, and a reflection on the ethical and ecological implications. This section is where theory becomes practice — where intelligence is tested, measured, and shaped into something useful, sustainable, and human‑centered."
  %}
</section>

---

<!-- PROJECT FEED -->
<section class="project-feed">

  <h2 class="feed-title">Projects</h2>

  <div class="project-feed-scroll">

{% assign projects = site["applied-works"] | group_by: "project" %}
    {% for project in projects %}
      {% assign posts = project.items %}
      {% assign intro = posts | where: "type", "intro" | first %}
      {% assign tech = posts | where: "type", "technical" | first %}
      {% assign ethics = posts | where: "type", "ethical" | first %}
      {% include project-card.html
         thumbnail=intro.thumbnail
         title=project.name
         resume=intro.resume
         intro=intro.url
         tech=tech.url
         ethics=ethics.url
      %}
    {% endfor %}

  </div>

</section>
