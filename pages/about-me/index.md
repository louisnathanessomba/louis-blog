---
layout: section
title: "About Me"
subtitle: "Identity, Mission & Journey"
permalink: /about-me/
---

<!-- HERO -->
<section class="section-hero">
  {% include hero.html
     portrait="/assets/images/me/formal.jpg"
     alt="Formal portrait of Louis Nathan Essomba"
     title=page.title
     subtitle=page.subtitle
     description="My name is Louis Nathan Essomba. I am a young scientist‑technologist exploring the frontier between devices, intelligence, ethics, and ecology. This blog is the living expression of my journey — a place where I document my research, my experiments, my reflections, and the philosophy behind the Firmware AI thesis. I believe that intelligence should be sustainable, local, transparent, and deeply human. Everything I build, write, or explore is guided by this conviction."
  %}
</section>

---

<!-- FEED (LATEST + MOST VIEWED) -->
<section class="section-feed">
  {% assign about_posts = site["about-me"] %}
  {% include feed.html
     title="Latest Personal Update"
     posts=about_posts
     most_viewed=""
     link="/about-me/"
     link_text="Browse all About Me →"
  %}
</section>

---

<!-- ALL POSTS -->
<section class="section-all-posts">
  <h2 class="feed-title">All About Me Posts</h2>

  {% assign all_about = site["about-me"] | sort: "date" | reverse %}
  {% for post in all_about %}
    {% include card.html
       thumbnail=post.thumbnail
       title=post.title
       resume=post.resume
       url=post.url
       cta="Read →"
    %}
  {% endfor %}
</section>
