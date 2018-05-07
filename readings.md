---
layout: store
title: "Tarot and Astrology"
---
<article class="store">

  <ul>
    {% for reading in site.readings %}
      <li>
        <a href="{{ reading.url }}">{{ reading.title }}</a>
        - {{ reading.price }}
      </li>
    {% endfor %}
  </ul>
</article>
