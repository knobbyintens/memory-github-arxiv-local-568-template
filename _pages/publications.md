---
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<h2>Publications</h2>

{% assign sorted_publications = site.publications | sort: "date" | reverse %}
{% for post in sorted_publications %}
  <div class="publication">
    <h3>{{ post.title }}</h3>
    <p class="pub-authors">{{ post.authors }}</p>
    <p class="pub-meta">{{ post.category }} &middot; {{ post.date | date: "%B %Y" }}</p>
    {% if post.arxiv %}
      <p><a href="https://arxiv.org/abs/{{ post.arxiv }}">arXiv:{{ post.arxiv }}</a></p>
    {% endif %}
  </div>
{% endfor %}
