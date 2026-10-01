---
layout: default
---

### அகக் களத் தியானம் | Inward Contemplations

<ul class="post-list" style="list-style-type: none; padding-left: 0;">
  {% for post in site.posts %}
    <li style="margin-bottom: 1.5rem;">
      <span class="post-meta" style="color: #666; font-size: 0.9em;">{{ post.date | date: "%B %d, %Y" }}</span>
      <h3 style="margin-top: 0.2rem;">
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h3>
      {% if post.excerpt %}
        <div style="font-size: 0.95em; color: #444;">{{ post.excerpt | strip_html | truncatewords: 30 }}</div>
      {% endif %}
    </li>
  {% endfor %}
</ul>
