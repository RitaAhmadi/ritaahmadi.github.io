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

  {% assign news_items = site.news | where: "inline", true | sort: "date" | reverse %}

  {% for post in news_items %}
    <div class="news-item">
      <p class="date">{{ post.date | date: "%Y-%m-%d" }}</p>
      <div class="content">
        {{ post.content }}
      </div>
    </div>
  {% endfor %}

</section>
