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

{% for post in site.publications reversed %}
  {% if post.type == 'journal' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## International Conference Papers

{% for post in site.publications reversed %}
  {% if post.type == 'proceedings' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## National Conference Papers
{% for post in site.publications reversed %}
  {% if post.type == 'natproceedings' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Thesis
{% for post in site.publications reversed %}
  {% if post.type == 'thesis' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
