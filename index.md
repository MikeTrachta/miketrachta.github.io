---
layout: default
---

<div class="home">
  <h1 class="page-heading">{{ page.title }}</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <h2>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h2>
        <div class="post-content">
          {{ post.content }}
        </div>
      </li>
    {% endfor %}
  </ul>
</div>