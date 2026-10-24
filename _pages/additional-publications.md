---
layout: page
permalink: /additional-publications/
title: other lab papers
description: publications by lab members not listed in Fred's publications page
nav: true
nav_order: 7
---

<!-- _pages/additional-publications.md -->

<div class="newpublications">

{% capture numOtherPapers %}
  {% bibliography_count --file other %}
{% endcapture %}

<div style="counter-reset:bibitem {{numOtherPapers|plus:1}}">
</div>
{% bibliography --file other --group_by year --group_order descending --template bib_other %}

</div>
