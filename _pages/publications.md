---
layout: page
permalink: /publications/
title: Publications
description: publications by categories in reversed chronological order. 
nav: true
nav_order: 3
---
<p style="margin-bottom: 1.5rem;">

Up-to-date publications are also available on 
<a href="https://scholar.google.com/citations?hl=en&user={{ site.data.socials.scholar_userid }}" 
   target="_blank" rel="noopener noreferrer">Google Scholar</a>.
</p>

<!-- _pages/publications.md -->
<div class="pub-note">
  <b>*</b> Indicates equal contribution. <u>Mentees</u> are underlined.  
  Peer-reviewed
</div>
<!-- Bibsearch Feature -->

<!-- {% include bib_search.liquid %} -->

<div class="publications">

<h2>Peer-reviewed Articles</h2>
{% bibliography -f papers -q @article %}

<h2>Manuscripts under review and in prep</h2>
{% bibliography -f papers -q @unpublished %}


</div>
