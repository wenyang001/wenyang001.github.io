---
layout: content_only
permalink: /publications/
title: Publications
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

{% include publication_list_style.html %}

<div class="publications">

{% bibliography %}

</div>

<script>
  (() => {
    const publications = document.querySelector('.content-only-page .publications');
    if (!publications) return;

    [...publications.querySelectorAll(':scope > h2.bibliography')].forEach((heading) => {
      const entries = heading.nextElementSibling;
      if (entries?.matches('ol.bibliography')) entries.after(heading);
    });
  })();
</script>
