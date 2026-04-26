---
layout: default
title: About
---

<section class="section-block">

<p class="section-label">About</p>

I am a researcher. blah blah 

</section>

<section class="section-block">

<p class="section-label">News</p>

{% assign sorted = site.news | sort: "date" | reverse %}

{% for item in site.news limit:10 %}
<div class="news-item">
  <div class="news-date">
    {{ item.date | date: "%Y-%m-%d" }}
  </div>

</div>
{% endfor %}
</section>
