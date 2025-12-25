---
layout: default
title: Home
permalink: /
nav: false
nav_order: 1
---

<div class="container mt-5">
  <div class="row align-items-center">
    
    <!-- Text Column -->
    <div class="col-md-7 text-center text-md-left">
      <div class="mb-4">
        <!-- Manually overriding header-bar styles by not using the class -->
        <h1 class="display-4" style="font-weight: 700; color: var(--global-theme-color);">Hi, I'm Ojasva.</h1>
        <h3 style="font-weight: 300; font-size: 1.5rem;">Undergraduate Researcher at P-square lab , IIT Roorkee.</h3>
      </div>

      <div class="lead mb-4" style="font-size: 1.1rem; line-height: 1.6;">
        <p>
          I am interested in <strong>Generative Models</strong> and <strong>Mechanistic Interpretability</strong>.
          <br>
          Currently working on sparsity-aware VAEs at P-Square Lab.
        </p>
      </div>

      <div class="cta-buttons mb-4">
        <a href="{{ '/work/' | relative_url }}" class="btn btn-primary mr-2" role="button">View My Work</a>
        <a href="{{ '/about/' | relative_url }}" class="btn btn-outline-primary" role="button">More About Me</a>
      </div>

      <!-- Social Links -->
      <div class="social-links text-md-left" style="font-size: 1.5rem;">
        <div class="contact-icons">
          {% include social.liquid %}
        </div>
      </div>
    </div>

    <!-- Image Column -->
    <div class="col-md-5 text-center">
      <div class="profile-container">
        <img 
          src="{{ '/assets/img/profile_pic.jpg' | relative_url }}" 
          alt="profile picture" 
          class="img-fluid" 
          style="
            border-radius: 20px; 
            box-shadow: 0 10px 30px -10px rgba(0,0,0,0.5); 
            max-width: 300px;
            object-fit: cover;
          "
        >
      </div>
    </div>

  </div>
</div>
