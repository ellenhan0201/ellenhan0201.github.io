---
layout: about
title: About
permalink: /
subtitle: Research scientist studying emotion, mental health, and AI through large-scale behavioral data, computational modeling, and visualization.

profile:
  align: right
  image: EllenHan.jpg
  image_circular: false # crops the image to make it circular
  # more_info: >
  #   <p>555 your office number</p>
  #   <p>123 your address street</p>
  #   <p>Your City, State 12345</p>

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 6 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<style>
  .post-header {
    margin-bottom: 1.9rem;
  }

  .post-header .desc {
    max-width: 58rem;
    margin-top: 0.55rem;
    margin-bottom: 0;
    color: var(--global-text-color-light);
    font-size: 1.08rem;
    line-height: 1.6;
  }

  .home-intro {
    max-width: 58rem;
    margin-bottom: 1.15rem;
  }

  .home-intro p {
    margin-bottom: 1.45rem;
    line-height: 1.58;
  }

  .home-intro p:last-child {
    margin-bottom: 0;
  }

  .home-intro .home-greeting {
    margin-bottom: 1.15rem;
    font-weight: 500;
  }

  .home-intro .home-section-label {
    margin-top: 2rem;
    margin-bottom: 0.5rem;
    line-height: 1.35;
  }

  .home-intro .home-expertise-list,
  .home-intro .home-work-list {
    margin-top: 0;
    padding-left: 1.2rem;
    line-height: 1.55;
  }

  .home-intro .home-expertise-list {
    margin-bottom: 1.8rem;
  }

  .home-intro .home-work-list {
    margin-bottom: 0;
  }

  .home-intro .home-expertise-list li,
  .home-intro .home-work-list li {
    margin-bottom: 0.28rem;
  }

  .home-intro .home-selected-work {
    max-width: 54rem;
    margin-top: 1.75rem;
    padding-top: 1.05rem;
    border-top: 1px solid var(--global-divider-color);
  }

  .home-intro .home-selected-work .home-section-label {
    margin-top: 0;
  }

  .post article > h2 {
    margin-top: 1.8rem;
    margin-bottom: 1.15rem;
    font-size: 1.65rem;
    line-height: 1.3;
  }

  .post article > h2 a:hover {
    text-decoration: none;
  }

  .news .table {
    margin-bottom: 1.8rem;
  }

  .news .table th,
  .news .table td {
    padding-top: 0.65rem;
    padding-bottom: 0.65rem;
    vertical-align: top;
  }

  .news .table th {
    white-space: nowrap;
  }

  @media (min-width: 576px) {
    .post .profile.float-right {
      margin-top: 0.35rem;
      margin-left: 2rem;
      margin-bottom: 1rem;
    }
  }

  @media (max-width: 575.98px) {
    .post-header .desc {
      font-size: 1rem;
    }

    .post article > h2 {
      font-size: 1.45rem;
    }

    .home-intro {
      margin-top: 1.5rem;
    }
  }
</style>

<div class="home-intro">
  <p class="home-greeting">Hello! This is Yanting Han.</p>

  <p>I study emotions, individual differences, and mental health by combining large-scale behavioral data collection, computational modeling, and interactive visualization. My research asks how subjective experiences are structured, how they vary across people, and how those insights can inform mental health and human-centered AI.</p>

  <p class="home-section-label"><strong>Industry-Relevant Expertise</strong></p>
  <ul class="home-expertise-list">
    <li>Large-scale behavioral data collection</li>
    <li>Computational modeling of emotion and individual differences</li>
    <li>Machine learning, dimensionality reduction, and visualization</li>
    <li>Mental health, affective science, and human-AI relevance</li>
    <li>Open science, data curation, and reproducible research</li>
  </ul>

  <div class="home-selected-work">
    <p class="home-section-label"><strong>Selected work</strong></p>
    <ul class="home-work-list">
      <li><a href="{{ '/projects/Emotion-Dim/' | relative_url }}">Dimensional Space of Human Emotions</a> maps subjective emotion experience across narratives, videos, and real-life reports.</li>
      <li><a href="{{ '/projects/COVID-Dynamic/' | relative_url }}">COVID-Dynamic Longitudinal Study</a> tracks psychological change during the COVID-19 pandemic through longitudinal behavioral data and public research resources.</li>
    </ul>
  </div>
</div>
