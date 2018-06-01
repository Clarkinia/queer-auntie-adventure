---
layout: shelf
title:
header: zodiac bag
subhead: Tarot & Astrology
author: with Regina Clarkinia
cta:
bgimage: store_home_bg_Nns5mNuCR5RvXpVzlbt1kgvyXgFak7tFcBOYDVshslY.jpg
---
<body>
<article class="store">
  <div class="store-items">
    <ul>
      {% for reading in site.readings %}
      <li>
        <a href="{{ reading.url }}">
        <div class="store-top">
          <div class="store-button">
            <img src="{{ site.github.url }}/assets/img/{{ reading.button }}" >
          </div>
          <div class="store-byline">
            <h8>{{ reading.byline }}</h8>
          </div>
          <div class ="store-whatuget">
            <h15>{{ reading.content }}</h15>
          </div>
          <div class="store-cta-button">
            <h15>{{ reading.cta }}</h15>
          </div>
          <div class="store-testimonial">
            <h15>"{{ reading.testimonial }}" —{{ reading.testimonial-auth}}</h15>
          </div>
        </div> <!-- closes store-top -->
        </a>
      </li>
      {% endfor %}
    </ul>
  </div><!-- closes store-items -->
</article>
</body>
