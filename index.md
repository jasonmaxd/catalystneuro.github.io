---
layout: splash
permalink: /
hidden: true
title: "<span style='text-align: center; font-family: Andale Mono, monospace; font-stretch: ultra-condensed; margin-bottom: 10px; font-weight: normal;'>CATALYST</span><br><span style='text-align: center; font-family: Arial, sans-serif;'>NEURO</span>"
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/splash_banner.jpeg
display_footer_image: true
excerpt: >
  <span style='font-family: Verdana, sans-serif;'>Data and software engineering solutions<br />for neuroscience labs</span>
feature_row:
  - image_path: /assets/images/Our-Mission.jpg 
    excerpt: "We believe that the future of neuroscience will be driven by collaboration between labs. Our mission is to develop channels of communication and distribution of resources between labs to enable exponential growth and innovation. We are at the forefront of this effort, shaping the way data, analysis and visualization tools are standardized and shared across the international community of systems neuroscientists. We ensure that these tools accelerate scientific discovery by working in parallel with neuroscientists and work with them to enhance the tools they already use."
    title: "<span style='font-family: Verdana, sans-serif; margin-bottom: 10px; font-weight: normal;'>Our <b>Mission</b></span>"
    url: "/mission/"
    btn_class: "btn--primary"
    btn_label: "<span style='font-family: Helvetica, sans-serif;'>Learn more</span>"
feature_row_gallery:
  - title: "Our Portfolio"
    excerpt: "We help neuroscientists utilize state-of-the-art tools in data analysis, visualization, organization, sharing, and publishing."
---

{% include feature_row type="left" %}
{% for feature in page.feature_row_gallery %}
  <div class="feature-row">
    <h2>{{ feature.title }}</h2>
    <p>{{ feature.excerpt }}</p>
    <div class="image-grid">
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-1.jpg' }}" alt="Image 1">
        <div class="image-overlay">
          <div class="image-overlay-content">
            <p>{{ feature.image_excerpts[0] }}</p>
            <a href="{{ '/project/dandi/' }}" class="btn {{ feature.btn_classes[0] }}">Learn More</a>
          </div>
        </div>
      </div>
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-2.jpg' }}" alt="Image 2">
        <div class="image-overlay">
          <div class="image-overlay-content">
            <p>{{ feature.image_excerpts[1] }}</p>
            <a href="{{ feature.image_links[1] }}" class="btn {{ feature.btn_classes[1] }}">{{ feature.btn_labels[1] }}</a>
          </div>
        </div>
      </div>
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-3.jpg' }}" alt="Image 1">
        <div class="image-overlay">
          <div class="image-overlay-content">
            <p>{{ feature.image_excerpts[0] }}</p>
            <a href="{{ feature.image_links[0] }}" class="btn {{ feature.btn_classes[0] }}">{{ feature.btn_labels[0] }}</a>
          </div>
        </div>
      </div>
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-4.jpg' }}" alt="Image 2">
        <div class="image-overlay">
          <div class="image-overlay-content">
            <p>{{ feature.image_excerpts[1] }}</p>
            <a href="{{ feature.image_links[1] }}" class="btn {{ feature.btn_classes[1] }}">{{ feature.btn_labels[1] }}</a>
          </div>
        </div>
      </div>
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-5.jpg' }}" alt="Image 1">
        <div class="image-overlay">
          <div class="image-overlay-content">
            <p>{{ feature.image_excerpts[0] }}</p>
            <a href="{{ feature.image_links[0] }}" class="btn {{ feature.btn_classes[0] }}">{{ feature.btn_labels[0] }}</a>
          </div>
        </div>
      </div>
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-6.jpg' }}" alt="Image 2">
        <div class="image-overlay">
          <div class="image-overlay-content">
            <p>{{ feature.image_excerpts[1] }}</p>
            <a href="{{ feature.image_links[1] }}" class="btn {{ feature.btn_classes[1] }}">{{ feature.btn_labels[1] }}</a>
          </div>
        </div>
      </div>
    </div>
  </div>
{% endfor %}
