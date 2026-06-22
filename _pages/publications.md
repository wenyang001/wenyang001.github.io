---
layout: page
permalink: /publications/
title: Publications
description: Selected publications in computer vision, image restoration, and multimodal AI.
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<style>
  .publications .rankings {
    display: flex;
    flex-wrap: wrap;
    gap: 0.35rem;
    margin: 0.25rem 0 0.35rem;
  }

  .publications .ranking-badge {
    display: inline-flex;
    align-items: center;
    padding: 0.1rem 0.45rem;
    border-radius: 999px;
    font-size: 0.72rem;
    font-weight: 600;
    line-height: 1.4;
    letter-spacing: 0;
    white-space: nowrap;
  }

  .publications .ranking-ccf {
    border: 1px solid rgba(198, 0, 180, 0.32);
    color: var(--global-theme-color);
    background: rgba(198, 0, 180, 0.07);
  }

  .publications .ranking-cas {
    border: 1px solid rgba(0, 0, 0, 0.15);
    color: var(--global-text-color);
    background: rgba(0, 0, 0, 0.035);
  }
</style>

<div class="publications">

{% bibliography %}

</div>
