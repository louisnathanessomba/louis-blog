---
layout: section
title: "Companies Threads"
subtitle: "Visions, Strategies & Technological Philosophies"
permalink: /exploring-frontiers/companies-threads/
---

<!-- HERO -->
<section class="section-hero">
  {% include hero.html
     portrait="/assets/images/me/thinking.jpg"
     alt="Louis Nathan Essomba analyzing technology companies"
     title=page.title
     subtitle=page.subtitle
     description="Companies Threads is where I analyze the strategies, architectures, and philosophies of major technology companies. Each thread is a deep dive into how these organizations think about intelligence, sustainability, data, devices, and the future of computing. This subsection helps me compare their visions with the Firmware AI thesis, revealing alignments, divergences, and lessons that shape my own work."
  %}
</section>

---

<!-- FEED (LATEST + MOST VIEWED) -->
<section class="section-feed">
  {% assign ct_posts = site["exploring-frontiers"] | where: "subsection", "companies-threads" %}
  {% include feed.html
     title="Latest Company Threads"
     posts=ct_posts
     most_viewed="microsoft-vs-google"
     link="/exploring-frontiers/companies-threads/"
     link_text="Browse all Company Threads →"
  %}
</section>

---

<!-- ALL POSTS -->
<section class="section-all-posts">
  <h2 class="feed-title">All Company Threads</h2>

  {% assign all_ct = site["exploring-frontiers"] | where: "subsection", "companies-threads" | sort: "date" | reverse %}
  {% for post in all_ct %}
    {% include card.html
       thumbnail=post.thumbnail
       title=post.title
       resume=post.resume
       url=post.url
       cta="Read →"
    %}
  {% endfor %}
</section>
