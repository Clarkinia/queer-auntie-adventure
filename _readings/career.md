---
name: Career Chart
price: 150
slug: career-chart
sku: ASTcar
image: store_career_noun_1502690_cc.svg
max: 1
byline: I am ready for a career game plan.
layout: default
description: The Career Chart looks what roles you perform in the workplace, how to capitalize on your talents and how you gain status, success and prominence.
how: How I devised this.
what: PDF and 1-Hour Consultation
testimonial: Regina helped me realize where my power was for my career, how to best handle issues that arise in that domain, and what to simply not worry about anymore.
options:
  - 10-minute phone follow-up session a week after the session.
button: store_buttons_career.jpg
cta: Order a career astrology chart
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
