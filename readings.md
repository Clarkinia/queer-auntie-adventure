---
layout: default
title:
---
<article class="store">
  <div class="store-header">
    <h5>Choose a reading</h5>
      <p>Which of the following best describes your needs?</p>
  </div>
  <div class="store-items">
    <ul>
      {% for reading in site.readings %}
        <li>
          <a href="{{ reading.url }}">
          <img src="{{ site.github.url }}/assets/img/{{ reading.image }}" height="100" width="100">
          <h6>{{ reading.byline }}</h6>
          <p>{{ reading.price }}</p>
          </a>
        </li>
      {% endfor %}
    </ul>
  </div>
</article>
