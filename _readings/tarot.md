---
name: Tarot
price: 80
slug: tarot
sku: TAR1hr
image: store_tarot_noun_1479176_cc.svg
max: 1
byline: I want perspective on my current situation.
layout: default
description: Tarot Readings give you insight into what's going on in your life right now. Get practical advice and messages from your subconscious and higher guidance.
how: How I devised this.
what: 1-Hour Reading
options:
  - Astrology chart reference.
testimonial: The tarot reading you did for me turned out to be spot-on in ways I could never have imagined at that moment. Thank you for your insights and encouragement.
button: store_buttons_tarot.jpg
cta: Schedule a tarot reading
---
<!-- STORE -->
<div class="store-orderform">
  <form name="contact" method="POST" data-netlify="true" action="/thank_you.md">
    <p class="hidden">   <!--- This is to distract bots using .hidden in the _default CSS file-->
      <label>Don’t fill this out if you're human: <input name="bot-field"></label>
    </p>
    <p>
    <div class="reading-selector">
      <p>Choose a Reading<br>
        <input id="career" type="radio" name="reading" value="career"> Career Chart<label class="drinkcard-cc career" for="career"></label>

        <input id="natal" type="radio" name="reading" value="natal"> Natal Chart<label class="drinkcard-cc natal" for="natal"></label>

        <input id="tarot" type="radio" name="reading" value="tarot"> Tarot Reading<label class="drinkcard-cc tarot" for="tarot"></label>
      </p>
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
  <small><a href="https://github.com/rcotrina94/icons">
  &copy; Icons by @rcotrina94 on Github</a></small>
</div> <!--- clsoes out store-orderform -->
