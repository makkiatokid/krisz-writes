---
layout: page
title: The Garden
permalink: /garden.html
---

# The Garden 🌺

Stories organized by topic, not by time. These are the wildflowers that grow in different patches of the field.

<div style="margin-top: 2rem;">
{% for post in site.garden %}
  <article style="margin-bottom: 2rem; padding-bottom: 2rem; border-bottom: 1px solid #e5e7eb;">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div style="color: #6b7280; font-size: 0.9rem; margin: 0.5rem 0;">
      {% if post.categories %}
        {% for category in post.categories %}
          <span style="background: #f3f4f6; padding: 0.25rem 0.5rem; border-radius: 4px; margin-right: 0.5rem;">{{ category }}</span>
        {% endfor %}
      {% endif %}
    </div>
    <p>{{ post.excerpt }}</p>
    <a href="{{ post.url }}">Read more →</a>
  </article>
{% endfor %}
</div>
