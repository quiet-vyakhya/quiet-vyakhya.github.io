---
layout: default
---

### Inward Contemplations | அகக் களத் தியானம்
*Inward contemplations on Vedanta, poetry, and nuances of language.*
*வேதாந்தம், கவிதை, இன்ன பிற மொழிநடைகள் குறித்த அகக் களத் தியானம்.* 

---
<ul class="post-list" style="list-style-type: none; padding-left: 0; margin-top: 2rem;">
  {% for post in site.posts %}
    <li style="margin-bottom: 2rem; border-bottom: 1px solid #eee; padding-bottom: 1rem;">
      <span class="post-meta" style="color: #666; font-size: 0.9em;">{{ post.date | date: "%B %d, %Y" }}</span>
      <h3 style="margin-top: 0.3rem; margin-bottom: 0.5rem;">
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h3>
      {% if post.excerpt %}
        <div style="font-size: 0.95em; color: #444; line-height: 1.6;">{{ post.excerpt | strip_html | truncatewords: 30 }}</div>
      {% endif %}
    </li>
  {% endfor %}
</ul>
