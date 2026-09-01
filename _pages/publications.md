---
layout: page
permalink: /publications/
title: Publications
description: Publications in reverse chronological order.
years: [2026, 2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

Peer-reviewed articles and selected preprints are listed in reverse chronological order. For the complete record, including abstracts and conference contributions, see my [Google Scholar profile](https://scholar.google.com/citations?hl=en&user=uj3qcBkAAAAJ&view_op=list_works&sortby=pubdate).

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{ y }}</h2>
  {% bibliography -f papers -q @*[year={{ y }}]* %}
{% endfor %}

</div>
