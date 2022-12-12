---
layout: posts
permalink: /blog/
excerpt: "The blog for Optima Football"
title: Optima Football Blog
seo_title: "Optima Football Blog"
classes: wide
author_profile: true
---

A personal space sharing thoughts, opinions & news from the founder.

<h2>Latest updates on Optima Football</h2>

<div class="feature__wrapper">

{% assign site_posts = site.posts | sort: "last_modified_at" | reverse %}

{% if site_posts.size > 0 %}
  {% for post in site_posts limit:16 %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
{% endif %}

</div>
