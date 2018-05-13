---
layout: default
title:
---
<article class="store">
  <div class="store-header">
    <h7>Choose a reading</h7>
      <p>Which of the following best describes your needs?</p>
  </div>
  <div class="store-items">
    <ul>
      {% for reading in site.readings %}
        <li>
          <a href="{{ reading.url }}">
          <span class="store-images"><img src="{{ site.github.url }}/assets/img/{{ reading.image }}" height="80" width="80"></span>
          <h8>{{ reading.byline }}</h8>
          <p>{{ reading.price }}</p>
          </a>
        </li>
      {% endfor %}
    </ul>
  </div>
</article>
