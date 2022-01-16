---
layout: post
title:  "Images on this server"
date:   2021-12-24 12:01
categories: general test
---

This is an even older post for testing purposes ...

> A block quote
>

from [Jekyll documentation](https://jekyllrb.com/docs/static-files/)

{% assign image_files = site.static_files | where: "image", true %}

{% for myimage in image_files %}
  [{{ myimage.path }}]({{ myimage.path }} "an image")
{% endfor %}

{% for myimage in image_files %}
  ![]({{ myimage.path }} "an image")
{% endfor %}
