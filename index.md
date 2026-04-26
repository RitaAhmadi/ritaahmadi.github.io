---
layout: default
title: About
---

<section class="section-block">

<p class="section-label">About</p>

I am a researcher in quantum computation and quantum information theory.  
My work focuses on quantum complexity theory and the mathematical foundations of quantum computing.

</section>

<section class="section-block">

<p class="section-label">News</p>

{% assign sorted = site.news | sort: "date" | reverse %}

{% for item in sorted %}
  {% include news_item.html
    date=item.date
    text=item.content
  %}
{% endfor %}

</section>
