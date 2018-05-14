---
layout: default
title:
---
<body>
<article class="store">
  <div class="store-header">
    <h7>Choose a reading</h7>
      <div class="store-subhead">
        <br>
          <h9>[ Which of the following best describes you ]</h9>
      </div>
  </div>
  <div class="store-items">
    <ul>
      {% for reading in site.readings %}
        <li>
          <a href="{{ reading.url }}">
          <span class="store-images"><img src="{{ site.github.url }}/assets/img/{{ reading.image }}" height="80" width="80"></span>
          <h8>{{ reading.byline }}</h8>
          <br>{{ reading.content }}
          <br>{{ reading.price }}
          </a>
        </li>
      {% endfor %}
    </ul>
  </div>
  <div class="store-subhead">
    <br>
      <h9>[ How to reserve a reading with Regina ]</h9>
        <ul>
          <li><h8>Select your date and time</h8></li>
          <br><p>Submit your appointment details then pay to confirm your appointment.</p>
          <li><h8>More options</h8></li>
          <br><p>Do you want a different time than what is available or to check on last-minute openings?</p>
        </ul>
  </div>
  <div class="store-policy">
  <h8>24-hour No Show, Cancellation & Reschedule Policy</h8>
    <p>If you miss your appointment, cancel or reschedule with less than 24-hours notice, you will be charged the full fee. When you schedule an appointment, Regina reserves that time and space for you. If you make last-minute changes, it limits the chances for booking other clients. </p>
    </div>
</article>
<br>
<div class="attribution">
  <h4>Icons are designed by <a target="_blank" href="https://thenounproject.com/noomtah/"> Nithinan Tatah </a> and <a target="_blank" href="https://thenounproject.com/elki/"> Made.</a></h4>
</div>
</body>
