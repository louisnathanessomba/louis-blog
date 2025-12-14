---
layout: section
title: "Foundations"
subtitle: "Core Ideas & Vision"
permalink: /foundations/
---

<!-- HERO -->
<section class="section-hero">
  {% include hero.html
     portrait="/assets/images/me/conceptual.jpg"
     alt="Louis Nathan Essomba reflecting on ideas"
     title=page.title
     subtitle=page.subtitle
     description="Foundations is the conceptual core of my work. This is where the Firmware AI thesis is shaped, challenged, refined, and expanded. Here, I explore the principles that guide my entire vision: decentralization, sustainability, human‑centered intelligence, and the idea that technology should empower rather than dominate. These essays form the intellectual backbone of everything I build — the theory before the practice, the architecture before the code, the meaning before the mechanism."
  %}
</section>

---

<!-- FEED (LATEST + MOST VIEWED) -->
<section class="section-feed">
  {% assign foundation_posts = site["foundations"] %}
  {% include feed.html
     title="Core Essays"
     posts=foundation_posts
     most_viewed="firmware-ai-thesis"
     link="/foundations/"
     link_text="Browse all Foundations →"
  %}
</section>

---

<!-- ALL POSTS -->
<section class="section-all-posts">
  <h2 class="feed-title">All Foundations Posts</h2>

  {% assign all_foundations = site["foundations"] | sort: "date" | reverse %}
  {% for post in all_foundations %}
    {% include card.html
       thumbnail=post.thumbnail
       title=post.title
       resume=post.resume
       url=post.url
       cta="Read →"
    %}
  {% endfor %}
</section>
