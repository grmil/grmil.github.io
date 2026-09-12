---
icon: fas fa-tags
order: 3
---

<div id="post-list" class="flex-grow-1 px-xl-1">

  {% assign courses = site.courses | sort: "order" %}

  {% for course in courses %}
    <article class="card-wrapper card">
      <a href="{{ course.url | relative_url }}" class="post-preview row g-0 flex-md-row-reverse">

        <div class="col-md-12">
          <div class="card-body d-flex flex-column">

            <h1 class="card-title my-2 mt-md-0">
              {{ course.title }}
            </h1>

            {% if course.description %}
              <div class="card-text content mt-0 mb-3">
                <p>{{ course.description }}</p>
              </div>
            {% endif %}

            <div class="post-meta flex-grow-1 d-flex align-items-end">
              <div class="me-auto">
                <i class="fas fa-book fa-fw me-1"></i>
                Course
              </div>
            </div>

          </div>
        </div>

      </a>
    </article>
  {% endfor %}

</div>

### Fall 2026:
- CIS 452: Operating Systems
- CIS 291: Intro to Computing Research
- HNR 300: Community Engagement
- MTH 350: Modern Algebra
- STA 412: Mathematical Statistics
