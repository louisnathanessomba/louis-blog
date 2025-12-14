---
layout: section
title: "Chemistry"
subtitle: "Transformation, Structure & Emergence"
permalink: /exploring-frontiers/independently-search/chemistry/
---

<!-- HERO -->
<section class="section-hero">
  {% include hero.html
     portrait="/assets/images/me/thinking.jpg"
     alt="Louis Nathan Essomba reflecting on chemistry"
     title=page.title
     subtitle=page.subtitle
     description="Chemistry is the science of change — the study of how matter transforms, interacts, and organizes itself into increasingly complex structures. In this subsection, I explore the molecular principles that shape everything from materials to biological systems. These ideas help me understand emergence, energy flow, and the physical constraints behind sustainable computation — essential insights for the Firmware AI thesis."
  %}
</section>

---

<!-- FEED (LATEST + MOST VIEWED) -->
<section class="section-feed">
  {% assign chem_posts = site["exploring-frontiers"] | where: "subsubsection", "chemistry" %}
  {% include feed.html
     title="Latest Chemistry Explorations"
     posts=chem_posts
     most_viewed="chemistry-example"
     link="/exploring-frontiers/independently-search/chemistry/"
     link_text="Browse all Chemistry →"
  %}
</section>

---

<!-- ALL POSTS -->
<section class="section-all-posts">
  <h2 class="feed-title">All Chemistry Posts</h2>

  {% assign all_chem = site["exploring-frontiers"] | where: "subsubsection", "chemistry" | sort: "date" | reverse %}
  {% for post in all_chem %}
    {% include card.html
       thumbnail=post.thumbnail
       title=post.title
       resume=post.resume
       url=post.url
       cta="Read →"
    %}
  {% endfor %}
</section>
