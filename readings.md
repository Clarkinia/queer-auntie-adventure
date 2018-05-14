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
    <form name="contact" method="POST" data-netlify="true" action="/thank_you.md">
      <p class="hidden">   <!--- This is to distract bots using .hidden in the _default CSS file-->
        <label>Don’t fill this out if you're human: <input name="bot-field"></label>
      </p>
      <p>
        <label>Select a Reading<br>
          <input type="radio" name="reading" value="career"> Career Chart<br>
          <input type="radio" name="reading" value="natal"> Natal Chart<br>
          <input type="radio" name="reading" value="tarot"> Tarot Reading<br>
        </label>
      </p>
      <p>
        <label>Your date of birth<br>
          <input type="birth-date" name="bday"><br>
        </label>
        <label>Your time of birth<br>
          <input type="birth-time" name="usr_time"><br>
        </label>
        <label>Where you were born
          <input type="text" name="birth-location" value="Country, City, State"><br>
        </label>
      </p>
      <p>
        <label>Your Name: <input type="text" name="name"></label>   
      </p>
      <p>
        <label>Your Email: <input type="email" name="email"></label>
      </p>
      <p>
        <label>Your Phone: <input type="tel" name="email"></label>
      </p>
      <p>
        <label>Message: <textarea name="message"></textarea></label>
      </p>
      <p>
        <button type="submit">Send</button>
      </p>
    </form>
  </div>
</article>
<br>
<div class="attribution">
  <h4>Icons are designed by <a target="_blank" href="https://thenounproject.com/noomtah/"> Nithinan Tatah </a> and <a target="_blank" href="https://thenounproject.com/elki/"> Made.</a></h4>
</div>
</body>
