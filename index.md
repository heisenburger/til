---
layout: default
---

<ul class="posts">
  {% assign entries = site.posts %}
  {% for entry in entries %}
      <li><a class="l-nu _hover _focus" href="{{ entry.url | prepend: site.baseurl }}"><small>{{ entry.date  | date: "%d/%m" }}</small>: {{ entry.title }}</a></li>
  {% endfor %}
</ul>

{% include nav.html %}