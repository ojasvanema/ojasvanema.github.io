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

  .cta-buttons {
    display: flex;
    flex-wrap: wrap;
    gap: 0.85rem;
  }

  .btn-action-primary {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 0.65rem 1.35rem;
    font-size: 0.95rem;
    font-weight: 500;
    letter-spacing: -0.01em;
    color: var(--global-bg-color) !important;
    background-color: var(--global-text-color);
    border: 1px solid var(--global-text-color);
    border-radius: 6px;
    text-decoration: none !important;
    transition: all 0.2s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .btn-action-primary:hover {
    background-color: var(--global-theme-color);
    border-color: var(--global-theme-color);
    color: #fff !important;
  }

  .btn-action-primary:hover .arrow,
  .btn-action-secondary:hover .arrow {
    transform: translateX(3px);
  }

  .btn-action-secondary {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 0.65rem 1.35rem;
    font-size: 0.95rem;
    font-weight: 500;
    letter-spacing: -0.01em;
    color: var(--global-text-color) !important;
    background-color: transparent;
    border: 1px solid var(--global-divider-color);
    border-radius: 6px;
    text-decoration: none !important;
    transition: all 0.2s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .btn-action-secondary:hover {
    border-color: var(--global-text-color);
    background-color: rgba(125, 125, 125, 0.06);
  }

  .arrow {
    display: inline-block;
    transition: transform 0.2s ease;
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
        <h3 class="font-weight-normal mt-3" style="font-size: 1.35rem; color: var(--global-text-color);">
          Research Engineer at <a href="https://elimentary.com/" target="_blank" style="color: inherit; text-decoration: underline; text-decoration-color: var(--global-theme-color); white-space: nowrap;">Elimentary</a>
        </h3>
        <p class="mt-2" style="font-size: 1.05rem; color: var(--global-text-color-light); font-weight: 400; line-height: 1.6;">
          Undergraduate Researcher at <a href="https://psquare-lab.github.io/" target="_blank" style="color: inherit; text-decoration: underline; text-decoration-color: var(--global-theme-color); white-space: nowrap;">P-Square Lab</a>, IIT Roorkee &bull; Research Intern at <a href="https://c-d-s.github.io/" target="_blank" style="color: inherit; text-decoration: underline; text-decoration-color: var(--global-theme-color); white-space: nowrap;">Yale University</a>
        </p>
      </div>

      <div class="lead mb-4" style="font-size: 1.15rem; line-height: 1.6; color: var(--global-text-color-light);">
        <p>
          Working on <strong style="color: var(--global-theme-color);">Causal Representation Learning</strong>,
          <strong>Deep Generative Models</strong>, and <strong>Mechanistic Interpretability</strong>.
        </p>
      </div>

      <div class="cta-buttons mb-5">
        <a href="{{ '/work/' | relative_url }}" class="btn-action-primary" role="button">
          <span>Selected Work</span>
          <span class="arrow">&rarr;</span>
        </a>
        <a href="{{ '/about/' | relative_url }}" class="btn-action-secondary" role="button">
          <span>About & Bio</span>
          <span class="arrow">&rarr;</span>
        </a>
      </div>

    </div>

    <!-- Image Column -->
    <div class="col-md-5 text-center">
      <div class="profile-container">
        <img 
          src="{{ '/assets/img/profile_pic.jpeg' | relative_url }}" 
          alt="Ojasva Nema" 
          class="img-fluid" 
          style="
            border-radius: 20px; 
            max-width: 320px;
            width: 100%;
            aspect-ratio: 1 / 1;
            object-fit: cover;
            border: 1px solid var(--global-divider-color);
            box-shadow: 0 12px 36px -8px rgba(0,0,0,0.18);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
          "
          onmouseover="this.style.transform='translateY(-3px)'; this.style.boxShadow='0 16px 44px -8px rgba(0,0,0,0.22)'"
          onmouseout="this.style.transform='translateY(0)'; this.style.boxShadow='0 12px 36px -8px rgba(0,0,0,0.18)'"
        >
      </div>
    </div>

  </div>
</div>
