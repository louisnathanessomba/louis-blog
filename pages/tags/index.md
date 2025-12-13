---
layout: section
title: "Tags"
subtitle: "Browse all topics"
permalink: /tags/
---

# All Tags

<ul class="tag-list">
  {% assign all_tags = site.tags | sort %}
  {% for tag in all_tags %}
    <li>
      <a class="tag" href="{{ '/tags/' | relative_url }}{{ tag[0] | slugify }}/">
        {{ tag[0] }} ({{ tag[1].size }})
      </a>
    </li>
  {% endfor %}
</ul>
