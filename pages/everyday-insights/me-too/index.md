---
layout: section
title: "Me Too"
subtitle: "Reflections Beyond the Framework"
permalink: /everyday-insights/me-too/
---

<!-- HERO -->
<section class="section-hero">
  {% include hero.html
     portrait="/assets/images/me/reflective.jpg"
     alt="Louis Nathan Essomba reflecting on life and news"
     title=page.title
     subtitle=page.subtitle
     description="Me Too is my free zone — the place where I write outside my core fields of science, engineering, and philosophy. Here, I share personal reflections, reactions to news, opinions on society, and thoughts that don’t fit neatly into the structure of my research. This subsection is spontaneous, honest, and human. It captures the moments where I step back from the work and simply express myself."
  %}
</section>

---

<!-- FEED (LATEST + MOST VIEWED) -->
<section class="section-feed">
  {% assign metoo_posts = site["everyday-insights"] | where: "subsection", "me-too" %}
  {% include feed.html
     title="Latest Reflections"
     posts=metoo_posts
     most_viewed="opinion-example"
     link="/everyday-insights/me-too/"
     link_text="Browse all Me Too posts →"
  %}
</section>

---

<!-- ALL POSTS -->
<section class="section-all-posts">
  <h2 class="feed-title">All Me Too Posts</h2>

  {% assign all_metoo = site["everyday-insights"] | where: "subsection", "me-too" | sort: "date" | reverse %}
  {% for post in all_metoo %}
    {% include card.html
       thumbnail=post.thumbnail
       title=post.title
       resume=post.resume
       url=post.url
       cta="Read →"
    %}
  {% endfor %}
</section>
