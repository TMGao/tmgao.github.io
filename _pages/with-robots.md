---
layout: page
title: "With Robots"
permalink: /with-robots/
author_profile: true
---

<h1>With Robots</h1>

<p>Here are some pictures of me with robots.</p>

{% for image in site.static_files %}
  {% if image.path contains 'images/robots' %}
    <img src="{{ site.baseurl }}{{ image.path }}" alt="Robot Image" style="width: 300px; margin: 10px;">
  {% endif %}
{% endfor %}

