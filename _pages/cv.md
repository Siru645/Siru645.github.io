---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

<!-- Embed the CV -->
{% assign bust = site.github.build_revision | default: site.time | date: "%s" %}
<iframe
  src="{{ '/files/CV_Zili.pdf' | relative_url }}?v={{ bust }}"
  width="80%"
  height="450"
  frameborder="0"
  marginwidth="0"
  marginheight="0">
</iframe>



<!--A PDF copy of my résumé is also available [here](/files/Resume_Zili.pdf).-->
