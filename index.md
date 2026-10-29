---
layout: page
title: Learn to lead AI transformation, one framework at a time
---

<p class="hero-lede">I'm working through a course on leading AI transformation. After each lesson I turn my
notes into a practical framework, show it working on a realistic case study, and publish it here so you can
use it too. No technical background needed.</p>

<p><a class="button" href="{{ site.posts.last.url | relative_url }}">Start with the introduction</a>
<a class="button button-secondary" href="{{ '/subscribe/' | relative_url }}">Get new lessons by email or RSS</a></p>

## How every lesson works

<div class="steps">
  <div class="step"><span class="step-num">1</span><strong>Key pointers</strong><br>The handful of ideas worth remembering.</div>
  <div class="step"><span class="step-num">2</span><strong>The framework</strong><br>Those ideas organised into something reusable.</div>
  <div class="step"><span class="step-num">3</span><strong>Case study</strong><br>The framework applied step by step to a realistic company.</div>
  <div class="step"><span class="step-num">4</span><strong>Putting it to work</strong><br>What to do with it in your own organisation.</div>
</div>

## Lessons

<ul class="lesson-list">
{% assign lessons = site.posts | where_exp: "p", "p.framework" | reverse %}
{% for post in lessons %}
  <li>
    <p class="lesson-module">{{ post.module }}</p>
    <a class="lesson-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <p class="lesson-fw">Framework: {{ post.framework }}</p>
    <p>{{ post.summary }}</p>
  </li>
{% endfor %}
</ul>

New here? Read [why I'm building this playbook]({{ site.posts.last.url | relative_url }}), then take the
lessons in order. They build on each other, and the case studies follow the same fictional company.

{% include subscribe.html %}
