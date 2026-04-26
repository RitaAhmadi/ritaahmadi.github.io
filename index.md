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

{% for item in sorted limit:10 %}
  <div class="news-item">
    <span class="news-date">
      {{ item.date | date: "%Y-%m-%d" }}
    </span>

    <span class="news-title">
      {{ item.title }}
    </span>
  </div>
{% endfor %}

</section>

