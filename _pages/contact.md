---
layout: default
title: Contact
permalink: /contact/
---

<div class="header-box">
  <h1>Contact Us</h1>
  <p>Feel free to reach out to us with any inquiries or questions.</p>
</div>

<div class="contact-info-box">
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-map-pin">
    <path d="M17.42 6.57l-5-3c-.47-.28-1.05-.28-1.42 0l-5 3C5.21 6.91 5 7.45 5 8v10c0 .55.45 1 1 1h10c.55 0 1-.45 1-1V8c0-.55-.21-1.09-.58-1.43z"></path>
    <path d="M12 22s-6-4.5-6-10.5 2.69-8.5 6-8.5S18 3.5 18 9.5 12 22 12 22z"></path>
  </svg>
  <p>
    844 Rose Drive, <br>
    Benicia, CA 94510
  </p>
</div>

<div class="contact-info-box">
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-mail">
    <path d="M22 3H2v18l20-18zM2 3h8l7 5 7-5h2v16H2z"></path>
  </svg>
  <p>inquiry@catalystneuro.com</p>
</div>

---

## Get in Touch

<form action="/submit-contact" method="POST">
  <div>
    <label for="first_name">First Name:</label>
    <input type="text" id="first_name" name="first_name" required>
    <label for="last_name">Last Name:</label>
    <input type="text" id="last_name" name="last_name" required>
  </div>
  <div>
    <label for="subject">Subject:</label>
    <input type="text" id="subject" name="subject" required>
  </div>
  <div>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
  </div>
  <div>
    <label for="message">Message:</label>
    <textarea id="message" name="message" required></textarea>
  </div>
  <div>
    <input type="submit" value="Submit">
  </div>
</form>