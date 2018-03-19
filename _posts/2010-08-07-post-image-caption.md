---
title: 'Post: Image (Caption)'
date: 2010-08-07 00:00:00 Z
categories:
- Post Formats
tags:
- image
- Post Formats
---

{% include base_path %}

{% capture fig_img %}
![Foo]({{ basepath }}/assets/images/unsplash-gallery-image-3.jpg)
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Photo from Unsplash.</figcaption>
</figure>