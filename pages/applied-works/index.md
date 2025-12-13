---
layout: section
title: "Applied Works"
subtitle: "Proofs of Concept"
permalink: /applied-works/
---

<!-- ============================================================
     SECTION HERO — PORTRAIT + MYTHIC SUBTITLE + DESCRIPTION
     ============================================================ -->
<section class="section-hero">

  <div class="section-hero-center">
 <img src="{{ '/assets/images/me/working.jpg' | relative_url }}"
         alt="Louis Nathan Essomba working on computer"
         class="section-portrait"
         loading="lazy">
<h1 class="section-title-hero">Applied Works</h1>
<p class="section-subtitle-hero">
      “Where ideas leave the page and become living systems.”
    </p>
<p class="section-description">
      Applied Works gathers all my real‑world experiments built from the Firmware AI thesis.
      Each project is a complete ecosystem: an introduction to the idea, a deep dive into the
      technical architecture, and a reflection on the ethical and ecological implications.
      This section is where theory becomes practice — where intelligence is tested, measured,
      and shaped into something useful, sustainable, and human‑centered.
    </p>

  </div>

</section>

---

<!-- ============================================================
     PROJECT FEED — SCROLLABLE, POLISHED, DYNAMIC
     ============================================================ -->
<section class="project-feed">

  <h2 class="feed-title">Projects</h2>

  <div class="project-feed-scroll">
 {% assign projects = site["applied-works"] | group_by: "project" %}
{% for project in projects %}
 {% assign posts = project.items %}
      {% assign intro = posts | where: "type", "intro" | first %}
      {% assign tech = posts | where: "type", "technical" | first %}
      {% assign ethics = posts | where: "type", "ethical" | first %}
<div class="project-card">
 <!-- Thumbnail / Asset -->
        {% if intro.thumbnail %}
          <img src="{{ intro.thumbnail | relative_url }}" class="project-thumb">
        {% else %}
          <img src="{{ '/assets/images/defaults/project.png' | relative_url }}" class="project-thumb">
        {% endif %}
<!-- Project Content -->
        <div class="project-content">
   <h3 class="project-title">{{ project.name }}</h3>
{% if intro.resume %}
            <p class="project-resume">{{ intro.resume }}</p>
          {% endif %}
<div class="project-links">
            {% if intro %}
              <a href="{{ intro.url | relative_url }}" class="project-link">Introduction →</a>
            {% endif %}
            {% if tech %}
              <a href="{{ tech.url | relative_url }}" class="project-link">Technical Details →</a>
            {% endif %}
            {% if ethics %}
              <a href="{{ ethics.url | relative_url }}" class="project-link">Ethical & Ecological →</a>
            {% endif %}
          </div>

 </div>
</div>

 {% endfor %}

  </div>

</section>
