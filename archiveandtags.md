---
layout: default
title: Tags
permalink: /tags/
---

<div class="tags">
  <h1 class="post-title">Tags</h1>

  <!--<ul class="tags">
    {% for tag in site.tags %}
      {% assign t = tag | first %}
      {% assign posts = tag | last %}
      <li>{{t | downcase | replace:" ","-" }} has {{ posts | size }} posts</li>
    {% endfor %}
  </ul>-->

 {% for tag in site.tags %}
      {% assign t = tag | first %}
      {% assign posts = tag | last %}
      {% if t != 'portfolio' and t != 'school' %}


        <h3>{{ t | downcase }}</h3>
        <ul>
          {% for post in posts %}
            {% if post.tags contains t %}
            <li>
              <a href="{{ post.url }}">{{ post.title }}</a>
              <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span> 
              <!-- <span class="date">{{ post.date | date: "%Y"  }}</span> -->
            </li>
           {% endif %}
          {% endfor %}
        </ul>

      {% endif %}
    {% endfor %}
  </div>