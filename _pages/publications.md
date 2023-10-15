---
layout: archive
title: "Papers"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<h2>Publications</h2>
{% for post in site.publications reversed %}
  {% if post.collection == 'publications' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Working Papers</h2>
{% for post in site.publications reversed %}
  {% if post.collection == 'workings' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
