---
title: Welcome to Simon's Digital Lab
layout: home
paginate: true
---

## Unraveling the Mysteries of AI in Medicine

Dive into a world where technology meets healthcare, explore groundbreaking research, and join me on a journey through the transformative landscape of Artificial Intelligence in medicine. Discover the potential, share the knowledge, and envision the future of healthcare with AI!

{% for post in paginator.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
{% endfor %}

<div class="pagination">
  <span class="previous">
    {% if paginator.previous_page %}
      <a href="{{ paginator.previous_page_path }}" class="previous">Previous</a>
    {% else %}
      <span class="previous disabled">Previous</span>
    {% endif %}
  </span>
  <span class="next">
    {% if paginator.next_page %}
      <a href="{{ paginator.next_page_path }}" class="next">Next</a>
    {% else %}
      <span class="next disabled">Next</span>
    {% endif %}
  </span>
</div>