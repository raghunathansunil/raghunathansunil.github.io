---
layout: page
title: Contact Us
permalink: /contactus/
---

<!-- modify this form HTML and place wherever you want your form -->
<p> Kindly send a message and problem statement with topic name to collaborate</p>
<form
  action="https://formspree.io/f/mpzokpdg"
  method="POST"
>
    <fieldset id="fs-frm-inputs">
        <label class="required" for="full-name">Full Name</label><br>
        <input type="text" name="name" id="full-name" size="104" required=""><br>
        <label class="required" for="email-address" >Email Address</label><br>
        <input type="text" name="_replyto" id="email-address" size="104" required><br>
        <label class="required" for="message">Message</label><br>
        <textarea name="message" id="message" rows="5" cols="100" required></textarea><br>
        <!-- your other form fields go here -->
        <input type="hidden" name="_subject" value="Github Comment!" />
        <input type="text" name="_gotcha" style="display:none" />
    </fieldset><br>
    <button type="submit">Send</button>

</form>

<p> The Contact form implemented with <a href="http://formspree.io"> formspree.io </a>. You will be redirected to ReCaptcha site.</p>