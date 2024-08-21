---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

## Journal Papers

{% for post in site.publications reversed %}{% if post.collection == 'publications' %}
  {% include archive-single.html %}
{% endif %}
{% endfor %}


## International Conference papers
{% for post in site.publications reversed %} {% if post.collection == 'conferences' %}
  {% include archive-single.html %}
{% endif %}
{% endfor %}

