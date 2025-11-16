---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

{% comment %} Job Market Paper {% endcomment %}
{% assign jmp = site.research | where: 'type', 'Job Market Paper' | sort: 'order_number' %}
{% if jmp.size > 0 %}
## Job Market Paper

{% for post in jmp %}
### {{ post.title }}

{% if post.links %}
{% for link in post.links %}
[{{ link.label }}]({{ link.url }}){% if forloop.last == false %} | {% endif %}
{% endfor %}
{% endif %}

{% if post.coauthors %}
<div class="coauthors"><em>{{ post.coauthors }}</em></div>
{% endif %}

<div class="abstract">
  {{ post.abstract | markdownify }}
</div>

{{ post.content | markdownify }}

{% endfor %}
{% endif %}

{% comment %} Work in Progress {% endcomment %}
{% assign wip = site.research | where: 'type', 'Work in Progress' | sort: 'order_number' %}
{% if wip.size > 0 %}
## Work in Progress

{% for post in wip %}
### {{ post.title }}

{% if post.links %}
{% for link in post.links %}
[{{ link.label }}]({{ link.url }}){% if forloop.last == false %} | {% endif %}
{% endfor %}
{% endif %}

{% if post.coauthors %}
<div class="coauthors"><em>{{ post.coauthors }}</em></div>
{% endif %}

<div class="abstract">
  {{ post.abstract | markdownify }}
</div>

{{ post.content | markdownify }}

{% endfor %}
{% endif %}