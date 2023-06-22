---
layout: splash
title: "Contact"
permalink: /contact/
feature_row:
  - image_path: /assets/images/c-banner-2.jpg
    alt: "Header Image"
    title: "Contact Us"
    excerpt: "We are ready to help your lab. Please send us a message below describing your needs and we would be happy to schedule a video call consultation."
    button_label: "Submit"
    button_url: "/submit-contact"
---


<div style="position: relative;">
  <div class="feature-row" style="background-image: url('{{ page.feature_row[0].image_path }}'); background-size: cover; background-position: center; display: flex;">
    <div class="header-content" style="flex-basis: 70%; color: #ffffff; padding: 4rem; position: relative;">
      <h1 style="font-size: 3rem; margin-left: 2rem;">
        <span style="position: relative;">
          <span class="color-line" style="position: absolute; left: -2rem; top: 50%; transform: translateY(-50%); width: 8px; height: 100%; background-color: #47e4e2;"></span>
          {{ page.feature_row[0].title }}
        </span>
      </h1>
      <p style="font-size: 1.5rem;">{{ page.feature_row[0].excerpt }}</p>
    </div>
    <div class="contact-info" style="flex-basis: 28%; display: flex; flex-direction: column; color: #ffffff justify-content: flex-end; padding: 4rem;">
      <h2 style="font-size: 2rem; color: #ffffff; margin-bottom: 1rem;">Contact Info</h2>
      <div style="display: flex; align-items: center; margin-bottom: 1rem;">
        <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 448 512">
          <path d="M400 32H48C21.49 32 0 53.49 0 80v352c0 26.51 21.49 48 48 48h352c26.51 0 48-21.49 48-48V80c0-26.51-21.49-48-48-48zM178.117 262.104C87.429 196.287 88.353 196.121 64 177.167V152c0-13.255 10.745-24 24-24h272c13.255 0 24 10.745 24 24v25.167c-24.371 18.969-23.434 19.124-114.117 84.938-10.5 7.655-31.392 26.12-45.883 25.894-14.503.218-35.367-18.227-45.883-25.895zM384 217.775V360c0 13.255-10.745 24-24 24H88c-13.255 0-24-10.745-24-24V217.775c13.958 10.794 33.329 25.236 95.303 70.214 14.162 10.341 37.975 32.145 64.694 32.01 26.887.134 51.037-22.041 64.72-32.025 61.958-44.965 81.325-59.406 95.283-70.199z"/>
        </svg>
        <p style="margin: 0 0 0 0.5rem;">Catalyst Neuro <br>844 Rose Drive, <br> Benicia, CA 94510</p>
      </div>
      <div style="display: flex; align-items: center;">
        <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 384 512">
          <path d="M172.268 501.67C26.97 291.031 0 269.413 0 192 0 85.961 85.961 0 192 0s192 85.961 192 192c0 77.413-26.97 99.031-172.268 309.67-9.535 13.774-29.93 13.773-39.464 0zM192 272c44.183 0 80-35.817 80-80s-35.817-80-80-80-80 35.817-80 80 35.817 80 80 80z"/>
        </svg>
        <p style="margin: 0 0 0 0.5rem;">inquiry@catalystneuro.com</p>
      </div>
    </div>
  </div>
</div>

## Get in Touch

<form action="{{ page.feature_row[0].button_url }}" method="POST">
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
    <input type="submit" value="{{ page.feature_row[0].button_label }}">
  </div>
</form>