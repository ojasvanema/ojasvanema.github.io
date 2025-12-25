---
layout: page
title: Work
permalink: /work/
nav: true
nav_order: 2
---

<!-- Research Experience Section -->
<h2 class="category">Research Experience</h2>
<div class="experience-section mb-5">
  
  <div class="job py-3 border-bottom">
    <div class="row">
      <div class="col-md-9">
        <h4 class="font-weight-bold">Undergraduate Researcher</h4>
        <h5 class="text-muted"><a href="https://psquare-lab.github.io/" target="_blank">P-Square Lab</a>, IIT Roorkee</h5>
      </div>
      <div class="col-md-3 text-md-right text-muted">
        <small>Present</small>
      </div>
    </div>
    <div class="mt-2">
      <p>
        Working with <a href="https://domingomery.ing.puc.cl/" target="_blank">Prof. Parikshit Pareek</a> on <strong>Deep Generative Models</strong>.
      </p>
      <ul>
        <li>Investigating <strong>Bilinear MLPs</strong> to design more interpretable neural architectures.</li>
        <li>Finalized a <strong>Sparse Diffusion</strong> framework for high-energy physics applications (CERN). <a href="https://drive.google.com/file/d/1gd-tJp-8napvR_qcfLp3wWk1FNH72SFo/view?usp=drive_link">[Read Paper]</a></li>
        <li>Designed a <strong>sparsity-aware Variational Autoencoder (VAE)</strong> for modeling data with only 0.2% active pixels, introducing a <strong>weighted loss</strong> to stabilize training.</li>
        <li>Building a foundation model for <strong>amortized kernel hyperparameter discovery</strong>.</li>
      </ul>
    </div>
  </div>



  <div class="job py-3 border-bottom">
    <div class="row">
      <div class="col-md-9">
        <h4 class="font-weight-bold">AI Engineer Intern</h4>
        <h5 class="text-muted"><a href="https://elimentary.com/" target="_blank">Elimentary</a></h5>
      </div>
      <div class="col-md-3 text-md-right text-muted">
        <small>Past</small>
      </div>
    </div>
    <div class="mt-2">
      <p>Gained production-grade AI experience working on Local LLMs.</p>
      <ul>
        <li>Engineered <strong>local LLM APIs</strong> to enable secure and efficient model deployment.</li>
        <li>Developed comprehensive <strong>evaluation pipelines</strong> to benchmark and validate model performance.</li>
        <li>Optimized workflows for production-ready AI systems.</li>
      </ul>
    </div>
  </div>

</div>


<!-- Publications Section -->
<h2 class="category mt-5">Publications</h2>
<div class="publications">
{% include selected_papers.liquid %}
</div>


<!-- Projects Section -->
<h2 class="category mt-5">Projects</h2>
<div class="projects">
{% include projects.liquid %}
</div>
