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

{% bibliography --group_by none %}

</div>

<script>
  (() => {
    const selfName = 'Wenyang Liu';

    const highlightSelf = (element) => {
      if (element.querySelector('.self-author')) return;

      const text = element.textContent;
      const selfIndex = text.indexOf(selfName);
      if (selfIndex < 0) return;

      const self = document.createElement('strong');
      self.className = 'self-author';
      self.textContent = selfName;
      element.replaceChildren(
        document.createTextNode(text.slice(0, selfIndex)),
        self,
        document.createTextNode(text.slice(selfIndex + selfName.length)),
      );
    };

    document.querySelectorAll('.publications .more-authors').forEach((element) => {
      const observer = new MutationObserver(() => highlightSelf(element));
      observer.observe(element, { childList: true, characterData: true, subtree: true });
      highlightSelf(element);
    });
  })();
</script>
