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
    title: "<span class='underlined-title'><span class='first-word'>Our</span> <b>Mission</b></span>"
    url: "/mission/"
    btn_class: "btn--primary"
    btn_label: "<span style='font-family: Helvetica, sans-serif;'>Learn more</span>"
feature_row_gallery:
  - title: "<span class='underlined-title'><span class='first-word'>Our</span> <b>Portfolio</b></span>"
    excerpt: "We help neuroscientists utilize state-of-the-art tools in data analysis, visualization, organization, sharing, and publishing."
feature_row_bottom:
  - title: "<span class='underlined-title'><span class='first-word'>Our</span> <b>Reach</b></span>"

---

{% include feature_row type="left" %}
{% for feature in page.feature_row_gallery %}

  <div class="feature-row">
    <h1>{{ feature.title }}</h1>
    <p>{{ feature.excerpt }}</p>
    <div class="image-grid">
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-1.jpg' }}" alt="Image 1">
        <div class="image-overlay">
          <div class="image-overlay-content">
          <div class="excerpt-line"></div>
            <p>DANDI<br>Massachusetts Institute of Technology</p>
            <a href="{{ '/project/dandi/' }}" class="btn {{ feature.btn_classes[0] }} custom-button-port">Learn More</a>
          </div>
        </div>
      </div>
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-2.jpg' }}" alt="Image 2">
        <div class="image-overlay">
          <div class="image-overlay-content">
          <div class="excerpt-line"></div>
            <p>Data Engineering Speech Neuroscience<br>UC San Francisco</p>
            <a href="{{ '/project/data-engineering-speech/' }}" class="btn {{ feature.btn_classes[1] }} custom-button-port">Learn More</a>
          </div>
        </div>
      </div>
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-3.jpg' }}" alt="Image 3">
        <div class="image-overlay">
          <div class="image-overlay-content">
          <div class="excerpt-line"></div>
            <p>Data Science Core of Ripple U19<br>Stanford University</p>
            <a href="{{ '/project/data-science-core/' }}" class="btn {{ feature.btn_classes[2] }} custom-button-port">Learn More</a>
          </div>
        </div>
      </div>
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-4.jpg' }}" alt="Image 4">
        <div class="image-overlay">
          <div class="image-overlay-content">
          <div class="excerpt-line"></div>
            <p>Data Standardization<br>Simons Foundation</p>
            <a href="{{ '/project/data-standardization/' }}" class="btn {{ feature.btn_classes[3] }} custom-button-port">Learn More</a>
          </div>
        </div>
      </div>
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-5.jpg' }}" alt="Image 5">
        <div class="image-overlay">
          <div class="image-overlay-content">
          <div class="excerpt-line"></div>
            <p>Interactive Data Visualization<br>Allen Institue and Kitware Inc.</p>
            <a href="{{ '/project/interactive-data/' }}" class="btn {{ feature.btn_classes[4] }} custom-button-port">Learn More</a>
          </div>
        </div>
      </div>
      <div class="image-grid-item">
        <img src="{{ '/assets/images/portfolio/slide-6.jpg' }}" alt="Image 6">
        <div class="image-overlay">
          <div class="image-overlay-content">
          <p class="excerpt-line"></p>
            <p>Neurodata Without Borders Dissemination<br>Lawrence Berkley National Laboratory</p>
            <a href="{{ '/project/nwb-dissemination/' }}" class="btn {{ feature.btn_classes[5] }} custom-button-port">Learn More</a>
          </div>
        </div>
      </div>
    </div>
  </div>
{% endfor %}
<hr style="margin-top: 40px; margin-bottom: 40px;">
{% for feature in page.feature_row_bottom %}
  <div class="feature-row">
    <h1 style="text-align: center;">{{ feature.title }}</h1>
    <div class="gif-container" style="display: flex; justify-content: center; align-items: center;">
      <img src="/assets/images/bottom.gif" alt="Bottom GIF">
    </div>
  </div>
{% endfor %}
