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
          <span class="store-images"><img src="{{ site.github.url }}/assets/img/{{ reading.image }}" height="80px" width="80px"></span>
          <h8>{{ reading.byline }}</h8>
          <br>{{ reading.content }}
          <br>{{ reading.price }}
          </a>
        </li>
      {% endfor %}
    </ul>
  </div>

    <br>
  <div class="store-orderform">
    <form name="contact" method="POST" data-netlify="true" action="/thank_you.md">
      <p class="hidden">   <!--- This is to distract bots using .hidden in the _default CSS file-->
        <label>Don’t fill this out if you're human: <input name="bot-field"></label>
      </p>




    <div class="cc-selector">

        <input id="visa" type="radio" name="credit-card" value="visa" />
        <label class="drinkcard-cc visa" for="visa"></label>

        <input id="mastercard" type="radio" name="credit-card" value="mastercard" />
        <label class="drinkcard-cc mastercard"for="mastercard"></label>

    </div>


<small><a href="https://github.com/rcotrina94/icons">
    &copy; Icons by @rcotrina94 on Github</a></small>

      <p>
      <div class="reading-selector">
        <label>Choose a Reading<br>
          <input id="career" type="radio" name="reading" value="career"> Career Chart<br>
          <input id="natal" type="radio" name="reading" value="natal"> Natal Chart<br>
          <input id="tarot" type="radio" name="reading" value="tarot"> Tarot Reading<br>
        </label>
      </div>
      </p>
      <p><label>Available Appointments<br>
        <select name="schedule-date-time">
        <option value="06/02/11:00am">Sat 6/2 @11:00am</option>
        <option value="06/02/12:30pm">Sat 6/2 @12:30pm</option>
        <option value="06/02/2:00pm">Sat 6/2 @2:00pm</option>

        <option value="06/04/11:00am">Mon 6/4 @11:00am</option>
        <option value="06/04/12:30pm">Mon 6/4 @12:30pm</option>
        <option value="06/04/2:00pm">Mon 6/4 @2:00pm</option>

        <option value="06/04/6:30pm">Mon 6/4 @6:30pm</option>
        <option value="06/04/8:00pm">Mon 6/4 @8:00pm</option>
        <option value="06/04/9:30pm">Mon 6/4 @9:30pm</option>
      </select>
      </label>
      </p>
      <p>
        <label>In-person readings take place in Hollywood, CA.<br>
        Phone Readings work just as well as face-to-face.<br>
          <input type="radio" name="reading" value="career"> Phone
          <input type="radio" name="reading" value="natal"> In-Person<br>
        </label>
      </p>
      <p>
        <label>Your date of birth<br>
          <input type="birth-date" name="bday"><br>
        </label>
        <label>Exact or Estimated or Don't Know time of birth<br>
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
  </div> <!--- clsoes out store-orderform -->
</article>
<br>
<div class="attribution">
  <h4>Icons designed by <a target="_blank" href="https://thenounproject.com/noomtah/"> Nithinan Tatah </a> and <a target="_blank" href="https://thenounproject.com/elki/"> Made.</a></h4>
</div>
</body>
