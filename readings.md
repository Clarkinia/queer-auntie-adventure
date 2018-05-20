---
layout: default
title:
---
<body>
<article class="store">
  <div class="store-header">
    <h7>Choose a reading</h7>
      <div class="store-subhead">
          <h9>Which of the following best describes you?</h9>
      </div>
  </div>
  <div class="store-items">
    <ul>
      {% for reading in site.readings %}
        <li>
          <a href="{{ reading.url }}">

          <div class="store-images"><img src="{{ site.github.url }}/assets/img/{{ reading.image }}" height="80px" width="80px"></div>

          <div class="store-top">
            <div class="store-byline">
              <h8>{{ reading.byline }}</h8>
            </div>
            <div class="store-description">
              <h15>{{ reading.description }}</h15>
            </div>
            <div class="store-whatuget">
              <h15> <span class="dollar-amt">{{ reading.what }}</span>
              </h15>
            </div>
            <div class="store-price">
              <h15>Price: <span class="dollar-amt">${{ reading.price }}</span></h15>
            </div>
          </div> <!-- closes store-top -->

          <div class="store-button">
          <h15>{{ reading.cta }}</h15>
          <img src="{{ site.github.url }}/assets/img/{{ reading.button }}" ></div>

          <div class="store-testimonial"><h16> <span class="dollar-amt">"{{ reading.testimonial }}"</span></h16></div>
          </a>
          <!--<hr>-->
        </li>
      {% endfor %}
    </ul>
  </div>
</article>
<br>
<div class="attribution">
<!--
  <h4>Icons designed by <a target="_blank" href="https://thenounproject.com/noomtah/"> Nithinan Tatah </a> and <a target="_blank" href="https://thenounproject.com/elki/"> Made.</a></h4>
  -->
</div>
</body>
