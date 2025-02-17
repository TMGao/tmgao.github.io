---
layout: page
title: "With Robots"
permalink: /with-robots/
author_profile: true
---

<h1>With Robots</h1>

<p>Here are some pictures of me with robots.</p>

<div class="gallery">
  {% for image in site.static_files %}
    {% if image.path contains 'images/robots' %}
      <div class="gallery-item">
        <img src="{{ site.baseurl }}{{ image.path }}" alt="Robot Image" style="width: 800px; margin: 10px;">
        <div class="caption">
          <!-- You can add your caption text here -->
          2021/05/09 I assembled the BlueROV2 for the first time and equipped it with a manipulator, successfully grabbing a hammer.
        </div>
      </div>
    {% endif %}
  {% endfor %}
</div>

<style>
  .gallery {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
  }

  .gallery-item {
    width: 300px;
    text-align: center;
    margin: 10px;
  }

  .gallery-image {
    width: 100%;
    height: auto;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  }

  .caption {
    margin-top: 10px;
    font-size: 14px;
    color: #555;
  }
</style>

