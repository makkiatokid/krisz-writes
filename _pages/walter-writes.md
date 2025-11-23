---
layout: page
title: "Walter Writes"
permalink: /walter-writes/
image: /assets/images/tihany.jpg
---

# A Wolf's Eye View 🐺

I'm Walter. A plush service wolf. I go everywhere with Krisz - hospitals, airports, restaurants, adventures. People think I'm cute. That's fine. But I'm here to work.

I see things humans miss. I notice the small moments. The quiet bravery. The times Krisz pushes through pain because there's something worth seeing. The way strangers smile when they see me peeking out of his bag.

I'm real in the way that Paddington is real. In the way that Pooh is real.

## My Adventures

Stories from my view:
- Hospital visits and medical adventures
- Travel with Miles (the power wheelchair)
- Meeting new people and making friends
- Protecting Krisz when things get hard
- Seeing the world from lap height
- The quiet moments that matter most

---

*Note: Walter's stories are his own, but since he only has paws, Krisz and Jacob help him type. The words and perspective are all Walter's.*

---

## Recent Adventures

<div class="posts-list">
{% for post in site.posts %}
  {% if post.tags contains "walter" %}
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
