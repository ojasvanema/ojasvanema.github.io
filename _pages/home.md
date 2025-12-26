---
layout: default
title: Home
permalink: /
nav: false
nav_order: 1
---

<style>
  /* Custom styles for the home page */
  .hero-container {
    min-height: 85vh;
    display: flex;
    align-items: center;
  }
  
  .gradient-text {
    background: linear-gradient(to right, var(--global-theme-color), #2a6f97);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-weight: 800;
  }

  .btn-theme {
    background-color: var(--global-theme-color);
    border-color: var(--global-theme-color);
    color: #fff;
    padding: 0.75rem 1.5rem;
    font-weight: 600;
    transition: all 0.3s ease;
  }

  .btn-theme:hover {
    background-color: var(--global-hover-color);
    border-color: var(--global-hover-color);
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  }

  .btn-outline-theme {
    color: var(--global-theme-color);
    border-color: var(--global-theme-color);
    background-color: transparent;
    padding: 0.75rem 1.5rem;
    font-weight: 600;
    transition: all 0.3s ease;
  }

  .btn-outline-theme:hover {
    background-color: var(--global-theme-color);
    color: #fff;
    transform: translateY(-2px);
  }

  .social-icon-link {
    color: var(--global-text-color-light);
    font-size: 1.8rem;
    margin-right: 1.2rem;
    transition: color 0.3s ease, transform 0.3s ease;
  }

  .social-icon-link:hover {
    color: var(--global-theme-color);
    transform: scale(1.1);
  }
</style>

<div class="container hero-container">
  <div class="row align-items-center w-100">
    
    <!-- Text Column -->
    <div class="col-md-7 text-center text-md-left">
      <div class="mb-4">
        <h1 class="font-weight-bold mb-3" style="font-size: 3.5rem; line-height: 1.2;">
          Hi, I'm <span class="gradient-text">Ojasva.</span>
        </h1>
        <h3 class="font-weight-light mt-3" style="font-size: 1.5rem; color: var(--global-text-color);">
          Undergraduate Researcher at <a href="https://psquare-lab.github.io/" target="_blank" style="color: inherit; text-decoration: underline; text-decoration-color: var(--global-theme-color); white-space: nowrap;">P-Square Lab</a>, IIT Roorkee.
        </h3>
      </div>

      <div class="lead mb-4" style="font-size: 1.15rem; line-height: 1.6; color: var(--global-text-color-light);">
        <p>
          I am interested in <strong style="color: var(--global-theme-color);">Generative Models</strong><br>
          and <strong>Mechanistic Interpretability</strong>.
          <br>
          Currently working on sparsity-aware VAEs.
        </p>
      </div>

      <div class="cta-buttons mb-5">
        <a href="{{ '/work/' | relative_url }}" class="btn btn-theme mr-3 rounded-pill" role="button">View My Work</a>
        <a href="{{ '/about/' | relative_url }}" class="btn btn-outline-theme rounded-pill" role="button">More About Me</a>
      </div>


    </div>

    <!-- Image Column -->
    <div class="col-md-5 text-center">
      <div class="profile-container position-relative">
        <div style="
          position: absolute;
          top: -15px;
          right: -15px;
          bottom: -15px;
          left: -15px;
          background: linear-gradient(135deg, var(--global-theme-color), transparent 60%);
          z-index: 0;
          border-radius: 40px;
          opacity: 0.2;
        "></div>
        <img 
          src="{{ '/assets/img/profile_pic.jpg' | relative_url }}" 
          alt="profile picture" 
          class="img-fluid position-relative z-depth-1" 
          style="
            border-radius: 30px; 
            max-width: 320px;
            width: 100%;
            object-fit: cover;
            z-index: 1;
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
          "
        >
      </div>
    </div>

  </div>
</div>
