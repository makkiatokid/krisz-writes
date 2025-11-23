---
layout: page
title: Archive
---

# Archive 📚

Browse all posts by date.

## All Posts

<div style="margin-top: 2rem;">
{% assign posts_by_year = site.posts | group_by_exp: "post", "post.date | date: '%Y'" %}
{% for year in posts_by_year %}
  <h3>{{ year.name }}</h3>
  <ul style="list-style: none; padding: 0;">
  {% for post in year.items %}
    <li style="margin-bottom: 1rem;">
      <span style="color: #6b7280;">{{ post.date | date: "%b %d" }}</span> - 
      <a href="{{ post.url }}">{{ post.title }}</a>
      {% if post.author %}<span style="color: #8b5cf6;"> by {{ post.author }}</span>{% endif %}
    </li>
  {% endfor %}
  </ul>
{% endfor %}
</div>
