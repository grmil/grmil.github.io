---
icon: fas fa-tags
order: 3
---

{% for post in site.posts %}
  <article class="card-wrapper">
    <a href="{{ post.url | relative_url }}" class="post-preview">
      <div class="card">
        <h2 class="card-title">{{ post.title }}</h2>

        {% if post.excerpt %}
          <p>{{ post.excerpt | strip_html | truncate: 200 }}</p>
        {% endif %}

        <small>
          {{ post.date | date: "%B %-d, %Y" }}
        </small>
      </div>
    </a>
  </article>
{% endfor %}

### Fall 2026:
- CIS 452: Operating Systems
- CIS 291: Intro to Computing Research
- HNR 300: Community Engagement
- MTH 350: Modern Algebra
- STA 412: Mathematical Statistics
