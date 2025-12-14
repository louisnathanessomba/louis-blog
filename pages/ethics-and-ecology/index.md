---
layout: section
title: "Ethics & Ecology"
subtitle: "Responsibility & Sustainability"
permalink: /ethics-and-ecology/
---

<!-- HERO -->
<section class="section-hero">
  {% include hero.html
     portrait="/assets/images/me/reflective.jpg"
     alt="Louis Nathan Essomba reflecting on ethics and ecology"
     title=page.title
     subtitle=page.subtitle
     description="Ethics & Ecology is the moral compass of my work. This section explores the responsibilities we carry as creators of intelligent systems: the ecological cost of computation, the ethical implications of automation, the balance between progress and preservation, and the duty to design technologies that respect both humanity and the planet. These essays form the conscience of the Firmware AI thesis — a reminder that innovation must remain sustainable, transparent, and deeply human."
  %}
</section>

---

<!-- FEED (LATEST + MOST VIEWED) -->
<section class="section-feed">
  {% assign ethics_posts = site["ethics-and-ecology"] %}
  {% include feed.html
     title="Ethical & Ecological Essays"
     posts=ethics_posts
     most_viewed="ethics-ecology-interdependence"
     link="/ethics-and-ecology/"
     link_text="Browse all Ethics & Ecology →"
  %}
</section>

---

<!-- ALL POSTS -->
<section class="section-all-posts">
  <h2 class="feed-title">All Ethics & Ecology Posts</h2>

  {% assign all_ethics = site["ethics-and-ecology"] | sort: "date" | reverse %}
  {% for post in all_ethics %}
    {% include card.html
       thumbnail=post.thumbnail
       title=post.title
       resume=post.resume
       url=post.url
       cta="Read →"
    %}
  {% endfor %}
</section>
