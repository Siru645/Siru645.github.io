---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
---

<!-- Embed the CV -->
{% assign bust = site.github.build_revision | default: site.time | date: "%s" %}
<iframe
  src="{{ '/files/CV_Siru.pdf' | relative_url }}?v={{ bust }}"
  width="80%"
  height="400"
  frameborder="0"
  marginwidth="0"
  marginheight="0">
</iframe>


## Resume

<iframe
  src="{{ '/files/Resume_Siru.pdf' | relative_url }}?v={{ bust }}"
  width="80%"
  height="400"
  frameborder="0"
  marginwidth="0"
  marginheight="0">
</iframe>

<!--A PDF copy of my résumé is also available [here](/files/Resume_Siru.pdf).-->
