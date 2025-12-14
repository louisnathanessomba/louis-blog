---
layout: section
title: "Computer Science"
subtitle: "Computation, Architecture & Intelligent Systems"
permalink: /exploring-frontiers/independently-search/computer-science/
---

<!-- HERO -->
<section class="section-hero">
  {% include hero.html
     portrait="/assets/images/me/thinking.jpg"
     alt="Louis Nathan Essomba thinking about computation"
     title=page.title
     subtitle=page.subtitle
     description="Computer Science is the study of computation, algorithms, and the architectures that make intelligent systems possible. In this subsection, I explore the principles behind software design, data structures, distributed systems, complexity, and the foundations of modern AI. These explorations directly feed into the Firmware AI thesis, helping me understand how to build systems that are efficient, local, sustainable, and aligned with human needs."
  %}
</section>

---

<!-- FEED (LATEST + MOST VIEWED) -->
<section class="section-feed">
  {% assign cs_posts = site["exploring-frontiers"] | where: "subsubsection", "computer-science" %}
  {% include feed.html
     title="Latest Computer Science Explorations"
     posts=cs_posts
     most_viewed="cs-example"
     link="/exploring-frontiers/independently-search/computer-science/"
     link_text="Browse all Computer Science →"
  %}
</section>

---

<!-- ALL POSTS -->
<section class="section-all-posts">
  <h2 class="feed-title">All Computer Science Posts</h2>

  {% assign all_cs = site["exploring-frontiers"] | where: "subsubsection", "computer-science" | sort: "date" | reverse %}
  {% for post in all_cs %}
    {% include card.html
       thumbnail=post.thumbnail
       title=post.title
       resume=post.resume
       url=post.url
       cta="Read →"
    %}
  {% endfor %}
</section>
