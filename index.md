---
layout: default
title: About
---

<section class="section-block">
  <p class="section-label">About</p>

  <div class="about-container">
    
    <!-- Photo -->
    <div class="about-photo">
      <img src="" alt="Profile photo">
    </div>

    <!-- Bio + Links -->
    <div class="about-text">
     <p> I am <strong>Rita Ahmadi</strong>; a stipendiary lecturer at Mansfield College, 
  <em>University of Oxford</em>. Before that, I was postdoctoral researcher at the 
  Department of Mathematics, <em>Imperial College London</em>. I did my 
  <em>DPhil</em> at Quantum Group based at the Department of Computer Science, 
  <em>University of Oxford</em>. During my PhD, I worked on topological quantum 
  computation and category theory. In my thesis, I studied and proposed 
  bicategorical structures for topological quantum computation. </p>

      <p class="social-links">
        <a href="https://scholar.google.com/citations?user=YOUR_ID" target="_blank">Google Scholar</a> ·
        <a href="https://bsky.app/profile/YOUR_HANDLE" target="_blank">Bluesky</a> ·
        <a href="https://www.linkedin.com/in/YOUR_PROFILE" target="_blank">LinkedIn</a> ·
        <a href="https://instagram.com/YOUR_HANDLE" target="_blank">Instagram</a>
      </p>

    </div>

  </div>
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
