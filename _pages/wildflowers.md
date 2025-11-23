---
layout: page
title: "Wildflowers"
permalink: /wildflowers/
image: /assets/images/las-vegas.jpg
---

# Every Wildflower Tells a Story 🌺

One moment, one story, told deeply and completely. This is my legacy - not journal entries, but real storytelling with photos from my perspective, showing you the world as I experience it.

Each chapter is one wildflower. One story. Told completely.

## What You'll Find Here

- **Cancer Chronicles**: Stage 4 colon cancer, pancreatic NET, surgeries, immunotherapy, the whole brutal journey
- **Diabetes Diaries**: Managing Type 1 diabetes (technically Type 3c) with my Dexcom CGM, insulin dosing 15x/day, hypo/hyper crises
- **Walter & Me**: Adventures with my plush service wolf who goes everywhere with me 🐺
- **Living with Incontinence**: Yes, I wear diapers 24/7 due to cerebral palsy. It's just my reality.
- **Fashion & Expression**: I'm a cisgender guy who doesn't believe clothing has gender rules. Fashion is self-expression, not gender assignment.
- **Food & Cooking**: Inventing and adapting recipes for my "mini-pan" (30% remaining pancreas)
- **Travel Stories**: Adventures with Miles (my power wheelchair) from Budapest to the UK and beyond
- **Growing Up Different**: Living with CP, being "different," finding myself
- **Medical Realities**: Procedures, hospital experiences, fighting for proper care
- **Relationships**: Family, friends, loneliness, connection, love in the time of dying
- **The Dark Stuff**: Fear, exhaustion, wondering if anyone will remember me

---

*Note: This site contains honest discussion of medical realities, disability experiences, and personal topics that some may find sensitive. I write from my authentic perspective as a cognitively young teenager navigating adult medical situations.*

---

## Recent Wildflowers

<div class="posts-list">
{% for post in site.posts %}
  {% if post.tags contains "wildflowers" %}
  <article class="post-item">
    <div class="post-item__content">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <time datetime="{{ post.date }}">{{ post.date | date: "%B %d, %Y" }}</time>
      {% if post.excerpt %}
        <p>{{ post.excerpt | strip_html | truncate: 200 }}</p>
      {% endif %}
    </div>
  </article>
  {% endif %}
{% endfor %}
</div>
