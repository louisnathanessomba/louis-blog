---
layout: section
title: "Student Life Tips"
subtitle: "Learning, Discipline & Daily Growth"
permalink: /everyday-insights/student-life-tips/
---

<!-- HERO -->
<section class="section-hero">
  {% include hero.html
     portrait="/assets/images/me/studying.jpg"
     alt="Louis Nathan Essomba studying"
     title=page.title
     subtitle=page.subtitle
     description="Student Life Tips is where I share the strategies, habits, and reflections that guide my daily life as a student in the scientific department. These notes are practical and honest — from study methods and time management to motivation, discipline, and the mental frameworks that help me grow. This subsection is the human engine behind my larger work: the routines that make the impossible possible."
  %}
</section>

---

<!-- FEED (LATEST + MOST VIEWED) -->
<section class="section-feed">
  {% assign slt_posts = site["everyday-insights"] | where: "subsection", "student-life-tips" %}
  {% include feed.html
     title="Latest Tips & Notes"
     posts=slt_posts
     most_viewed="study-methods-example"
     link="/everyday-insights/student-life-tips/"
     link_text="Browse all Student Life Tips →"
  %}
</section>

---

<!-- ALL POSTS -->
<section class="section-all-posts">
  <h2 class="feed-title">All Student Life Tips Posts</h2>

  {% assign all_slt = site["everyday-insights"] | where: "subsection", "student-life-tips" | sort: "date" | reverse %}
  {% for post in all_slt %}
    {% include card.html
       thumbnail=post.thumbnail
       title=post.title
       resume=post.resume
       url=post.url
       cta="Read →"
    %}
  {% endfor %}
</section>
