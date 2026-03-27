---
layout: page
title: Stephen Chen
description: A focused home for writing, experiments, and selected work.
cover: true
---

<div class="home-hero">
  <p class="home-kicker">Personal Site</p>
  <h2>A place for useful ideas, careful interface work, and the projects that survive first drafts.</h2>
  <p class="lead">I use this site to publish notes in progress, sharpen project writeups, and keep a stable public version of what I am making.</p>
  <div class="home-actions">
    <a class="home-button" href="/about/">About me</a>
    <a class="home-button secondary" href="/journal/">Read the journal</a>
    <a class="home-button ghost" href="https://github.com/siyche" rel="me noopener noreferrer">GitHub</a>
  </div>
</div>

<div class="home-grid">
  <section class="home-card">
    <p class="home-kicker">Current Focus</p>
    <h3>Small systems with strong defaults</h3>
    <p>I care about pages that stay clear under pressure: sensible structure, readable code, and details that still make sense six months later.</p>
  </section>
  <section class="home-card">
    <p class="home-kicker">Writing</p>
    <h3>Notes that do real work</h3>
    <p>The journal is for process notes, technical observations, and ideas worth turning into something more durable than a commit message.</p>
  </section>
  <section class="home-card">
    <p class="home-kicker">Intent</p>
    <h3>Less noise, more signal</h3>
    <p>This site should feel direct. A visitor should know what I care about, what I build, and where to go next within a few seconds.</p>
  </section>
</div>

<section class="home-section">
  <p class="home-kicker">Start Here</p>
  <div class="link-card-grid">
    <a class="link-card" href="/about/">
      <strong>About</strong>
      <span>A short biography, working style, and what this site is for.</span>
    </a>
    <a class="link-card" href="/journal/">
      <strong>Journal</strong>
      <span>Running notes, technical thoughts, and longer writing as it develops.</span>
    </a>
    <a class="link-card" href="https://github.com/siyche" rel="me noopener noreferrer">
      <strong>GitHub</strong>
      <span>Code, experiments, and the practical side of the work.</span>
    </a>
  </div>
</section>

{% if site.posts.size > 0 %}
<section class="home-section">
  <p class="home-kicker">Recent Writing</p>
  <ul class="home-list">
    {% for post in site.posts limit:3 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <small>{{ post.date | date: "%B %-d, %Y" }}</small>
      </li>
    {% endfor %}
  </ul>
</section>
{% endif %}

<section class="home-callout">
  <p class="home-kicker">Next Step</p>
  <p>Replace the starter copy with your actual bio, current work, and two or three project links. The structure is here now; the quality comes from the specifics you put into it.</p>
</section>
