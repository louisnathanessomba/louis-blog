---
layout: home
title: "Firmware AI — Responsible Innovation"
subtitle: "A living lab notebook by Louis Nathan Essomba"
permalink: /
---

# Welcome — I’m Louis Nathan Essomba

I’m a young scientist-technologist exploring the intersection of **AI, ethics, ecology, and device intelligence**.  
This blog is my **living lab notebook** — a place where I build, test, and refine the ideas behind my **Firmware AI thesis**.

Everything here is guided by a simple belief:

> **Intelligence should live on devices.  
> The cloud should be a library of algorithms, not a master.**

This homepage introduces my vision and guides you through the six divisions of the blog, each with its latest and most impactful posts.

---

# 🌌 My Vision

I imagine a world where:

- Devices carry **local intelligence**  
- The cloud becomes a **temporary algorithm library**  
- Innovation is **ethical, ecological, and equitable**  
- Technology respects **humans** and **Earth**  
- Access to algorithms is **democratized**, not centralized  

This blog is where I explore and build that future.

---

# 🧭 Explore the Blog  
### Six divisions — each with its latest and most viewed post

Below, each section includes:

✅ A short description  
✅ A link to the section  
✅ The **latest post**  
✅ The **most viewed post**  

---

# 📚 Foundations  
### Thesis & conceptual frameworks  
[Visit section →]({{ site.baseurl }}/foundations/)

{% assign f_posts = site.foundations | sort: "date" | reverse %}
{% assign f_latest = f_posts | first %}
{% assign f_most = site.foundations | sort: "views" | reverse | first %}

**Latest:**  
- [{{ f_latest.title }}]({{ site.baseurl }}{{ f_latest.url }})

**Most viewed:**  
- [{{ f_most.title }}]({{ site.baseurl }}{{ f_most.url }})

---

# 🛠 Applied Works  
### Real-world projects applying the thesis  
[Visit section →]({{ site.baseurl }}/applied-works/)

{% assign a_posts = site.applied-works | sort: "date" | reverse %}
{% assign a_latest = a_posts | first %}
{% assign a_most = site.applied-works | sort: "views" | reverse | first %}

**Latest:**  
- [{{ a_latest.title }}]({{ site.baseurl }}{{ a_latest.url }})

**Most viewed:**  
- [{{ a_most.title }}]({{ site.baseurl }}{{ a_most.url }})

---

# 🌌 Exploring Frontiers  
### Independent research & company vision threads  
[Visit section →]({{ site.baseurl }}/exploring-frontiers/)

{% assign e_posts = site.exploring-frontiers | sort: "date" | reverse %}
{% assign e_latest = e_posts | first %}
{% assign e_most = site.exploring-frontiers | sort: "views" | reverse | first %}

**Latest:**  
- [{{ e_latest.title }}]({{ site.baseurl }}{{ e_latest.url }})

**Most viewed:**  
- [{{ e_most.title }}]({{ site.baseurl }}{{ e_most.url }})

---

# 🌱 Ethics & Ecology  
### Responsibility at the core  
[Visit section →]({{ site.baseurl }}/ethics-and-ecology/)

{% assign ee_posts = site.ethics-and-ecology | sort: "date" | reverse %}
{% assign ee_latest = ee_posts | first %}
{% assign ee_most = site.ethics-and-ecology | sort: "views" | reverse | first %}

**Latest:**  
- [{{ ee_latest.title }}]({{ site.baseurl }}{{ ee_latest.url }})

**Most viewed:**  
- [{{ ee_most.title }}]({{ site.baseurl }}{{ ee_most.url }})

---

# 🎓 Everyday Insights  
### Student life tips & reflections on news  
[Visit section →]({{ site.baseurl }}/everyday-insights/)

{% assign i_posts = site.everyday-insights | sort: "date" | reverse %}
{% assign i_latest = i_posts | first %}
{% assign i_most = site.everyday-insights | sort: "views" | reverse | first %}

**Latest:**  
- [{{ i_latest.title }}]({{ site.baseurl }}{{ i_latest.url }})

**Most viewed:**  
- [{{ i_most.title }}]({{ site.baseurl }}{{ i_most.url }})

---

# 👤 About Me  
### Vision, background, and how to connect  
[Visit section →]({{ site.baseurl }}/about-me/)

{% assign me_posts = site.about-me | sort: "date" | reverse %}
{% assign me_latest = me_posts | first %}
{% assign me_most = site.about-me | sort: "views" | reverse | first %}

**Latest:**  
- [{{ me_latest.title }}]({{ site.baseurl }}{{ me_latest.url }})

**Most viewed:**  
- [{{ me_most.title }}]({{ site.baseurl }}{{ me_most.url }})

---

# ✅ How to Enable “Most Viewed”

Add this to each post’s front matter:

```yaml
views: 0
