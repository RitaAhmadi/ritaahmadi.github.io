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

  {% for post in site.news %}
    {% if post.inline %}
      <div class="news-item">
        <p class="date">{{ post.date | date: "%Y-%m-%d" }}</p>
        <div class="content">
          {{ post.content }}
        </div>
      </div>
    {% endif %}
  {% endfor %}

</section>

