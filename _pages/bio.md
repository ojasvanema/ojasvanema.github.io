---
layout: about
title: About
permalink: /about/
nav: true
nav_order: 3
subtitle: Undergraduate Researcher at <a href='https://psquare-lab.github.io/'>P-Square Lab</a>, IIT Roorkee.

profile:
  align: right
  image: 
  image_circular: false # crops the image to make it circular
  address: >
    <p>Department of Metallurgical and Materials Engineering</p>
    <p>IIT Roorkee, India</p>

news: false  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

Hi, I'm **Ojasva**.

I am an undergraduate at **IIT Roorkee** whose research spans **Causal Representation Learning**, **Deep Generative Models**, and **Mechanistic Interpretability**.

Previously, I was a **Research Intern at Yale University** with [Prof. Harsh Parikh](https://c-d-s.github.io/) (Causal Evidence & Decisions Studio), working on theoretical frameworks to construct Confidence Sets of Representations and causal representation learning.

At IIT Roorkee, I work at the [P-square Lab](https://psquare-lab.github.io/) with Prof. Parikshit Pareek, investigating **Bilinear MLPs** for architectural inductive bias and surgical unlearning, as well as building **foundation models for amortized kernel hyperparameter discovery** and physics-aware sparse diffusion models for CERN.

I also lead research on LLM internals at the [Data Science Group (DSG)](https://dsgiitr.in/), investigating how models route semantic domain knowledge (see our [preprint](https://drive.google.com/file/d/1jBVpFUeKDsRFVVz_b28iJ8kns9Y5E-9Z/view?usp=sharing) and [website](https://inside-llms.gitbook.io/surgical-domain-discovery)). Prior to this, I worked as a **Research Engineer at [Elimentary](https://elimentary.com/)** (YC F26) engineering quantized local LLM APIs and evaluation infrastructure, and developed [Image-Alchemy](https://arxiv.org/abs/2505.10743) (ICLR DeLTa workshop 2025).

Off the clock, I’m usually reading about finance (I’m always open to book recommendations!) or watching anime. Always happy to chat about circuits, LLMs, or what’s next in AI!

<style>
  .compute-status-dot {
    width: 8px;
    height: 8px;
    background-color: var(--global-theme-color);
    border-radius: 50%;
    display: inline-block;
    box-shadow: 0 0 8px var(--global-theme-color);
    animation: pulse-dot 2s infinite ease-in-out;
  }

  @keyframes pulse-dot {
    0%, 100% { transform: scale(1); opacity: 0.8; }
    50% { transform: scale(1.35); opacity: 1; }
  }

  .compute-step-btn {
    border: 1px solid var(--global-divider-color);
    background: transparent;
    color: var(--global-text-color-light);
    border-radius: 6px;
    padding: 0.35rem 0.75rem;
    font-size: 0.82rem;
    font-family: SFMono-Regular, Menlo, Monaco, Consolas, monospace;
    cursor: pointer;
    transition: all 0.2s ease;
  }

  .compute-step-btn:hover {
    border-color: var(--global-theme-color);
    color: var(--global-text-color);
  }

  .compute-step-btn.active {
    background-color: var(--global-theme-color);
    border-color: var(--global-theme-color);
    color: #ffffff !important;
    font-weight: 600;
  }

  .compute-step-btn.active sup {
    color: #ffffff !important;
  }

  .compute-terminal-box {
    transition: opacity 0.15s ease;
  }
</style>

<!-- Live "Infinite Compute" Micro-Widget -->
<div class="infinite-compute-widget my-5 p-4" style="border: 1px solid var(--global-divider-color); border-radius: 12px; background: var(--global-card-bg-color); box-shadow: 0 4px 20px -6px rgba(0,0,0,0.08);">
  
  <div class="d-flex justify-content-between align-items-center mb-3">
    <div class="d-flex align-items-center">
      <span class="compute-status-dot mr-2"></span>
      <span class="text-uppercase font-weight-bold" style="font-family: SFMono-Regular, Menlo, Monaco, Consolas, monospace; font-size: 0.78rem; letter-spacing: 0.08em; color: var(--global-theme-color);">
        Compute Speculation Matrix
      </span>
    </div>
    <div class="badge font-weight-normal px-2 py-1" style="font-family: SFMono-Regular, Menlo, Monaco, Consolas, monospace; font-size: 0.82rem; border: 1px solid var(--global-divider-color); color: var(--global-text-color);">
      Scale: <span id="compute-flops-badge" style="color: var(--global-theme-color); font-weight: 600;">10²⁶ FLOPs</span>
    </div>
  </div>

  <h5 class="font-weight-bold mb-2" style="font-size: 1.15rem; color: var(--global-text-color);">
    What would <em>you</em> do if you had infinite compute?
  </h5>
  
  <p class="text-muted mb-3" style="font-size: 0.92rem;">
    Explore speculative research horizons scaled across compute thresholds:
  </p>

  <!-- Interactive Step Dial -->
  <div class="compute-stepper mb-3 d-flex flex-wrap" style="gap: 0.5rem;">
    <button class="compute-step-btn" data-step="0">10<sup>22</sup> (Cluster)</button>
    <button class="compute-step-btn active" data-step="1">10<sup>26</sup> (Planetary)</button>
    <button class="compute-step-btn" data-step="2">10<sup>30</sup> (Dyson)</button>
    <button class="compute-step-btn" data-step="3">10<sup>40</sup> (Matrioshka)</button>
    <button class="compute-step-btn" data-step="4">&infin; (Asymptote)</button>
  </div>

  <!-- Speculation Terminal Display -->
  <div class="compute-terminal-box p-3 mb-4" style="border-radius: 8px; border: 1px solid var(--global-divider-color); background: rgba(125,125,125,0.05); font-family: SFMono-Regular, Menlo, Monaco, Consolas, monospace; font-size: 0.9rem; min-height: 75px; line-height: 1.6;">
    <span style="color: var(--global-theme-color); font-weight: bold;">$</span> <span id="compute-speculation-text">Loading speculation...</span>
  </div>

  <!-- Interactive User Response Box -->
  <div class="compute-reply-box">
    <label for="compute-user-input" class="text-muted mb-2" style="font-size: 0.85rem; font-family: SFMono-Regular, Menlo, Monaco, Consolas, monospace;">
      // What's your frontier answer?
    </label>
    <div class="input-group">
      <input type="text" id="compute-user-input" class="form-control" placeholder="e.g. Provably verify entire transformer circuit DAGs..." style="border-radius: 6px 0 0 6px; font-size: 0.9rem; border-color: var(--global-divider-color); background: var(--global-bg-color); color: var(--global-text-color);">
      <div class="input-group-append">
        <button class="btn btn-action-primary" id="compute-send-btn" type="button" style="border-radius: 0 6px 6px 0; padding: 0.5rem 1.1rem; font-size: 0.9rem;">
          <span>Send</span> <span class="arrow">&rarr;</span>
        </button>
      </div>
    </div>
    <small id="compute-send-feedback" class="text-success mt-2" style="display: none; font-family: SFMono-Regular, Menlo, Monaco, Consolas, monospace; font-size: 0.8rem;">
      &check; Opening email client to send your thought to Ojasva...
    </small>
  </div>

</div>

<script>
  (function() {
    const speculations = [
      {
        badge: "10²² FLOPs",
        text: "Exhaustively decompile every attention head and MLP sub-layer across 70B+ LLMs into human-verifiable algebraic operators; solve surgical domain unlearning without catastrophic forgetting."
      },
      {
        badge: "10²⁶ FLOPs",
        text: "Amortize Gaussian Process kernel hyperparameter discovery across all empirical sciences; train continuous-time neural ODEs directly on raw CERN LHC collision streams with zero structural bias."
      },
      {
        badge: "10³⁰ FLOPs",
        text: "Provably bound causal unidentifiability in non-linear dynamical systems by simulating counterfactual histories of the observable universe down to molecular granularity."
      },
      {
        badge: "10⁴⁰ FLOPs",
        text: "De novo simulation of complete cellular biology, neural morphogenesis, and quantum molecular mechanics in real time; compile entire synthetic organism genomes from first principles."
      },
      {
        badge: "∞ FLOPs",
        text: "Compute exact Kolmogorov complexity for all physical phenomena; generate provable mathematical truths across all formal systems; yet still debate whether transformers will ever be replaced."
      }
    ];

    const badgeEl = document.getElementById('compute-flops-badge');
    const textEl = document.getElementById('compute-speculation-text');
    const stepBtns = document.querySelectorAll('.compute-step-btn');
    const sendBtn = document.getElementById('compute-send-btn');
    const inputEl = document.getElementById('compute-user-input');
    const feedbackEl = document.getElementById('compute-send-feedback');

    function setStep(idx) {
      stepBtns.forEach(function(btn, i) {
        btn.classList.toggle('active', i === idx);
      });
      if (badgeEl) badgeEl.textContent = speculations[idx].badge;
      if (textEl) {
        textEl.style.opacity = '0';
        setTimeout(function() {
          textEl.textContent = speculations[idx].text;
          textEl.style.opacity = '1';
        }, 120);
      }
    }

    stepBtns.forEach(function(btn, idx) {
      btn.addEventListener('click', function() {
        setStep(idx);
      });
    });

    // Initialize with Step 1 (Planetary)
    setStep(1);

    if (sendBtn && inputEl) {
      sendBtn.addEventListener('click', function() {
        const val = inputEl.value.trim();
        if (!val) {
          inputEl.focus();
          return;
        }
        if (feedbackEl) feedbackEl.style.display = 'block';
        const subject = encodeURIComponent("If I had infinite compute...");
        const body = encodeURIComponent("Hey Ojasva,\n\nIf I had infinite compute, I would:\n" + val + "\n\nCheers!");
        window.location.href = "mailto:ojasva098@gmail.com?subject=" + subject + "&body=" + body;
      });

      inputEl.addEventListener('keydown', function(e) {
        if (e.key === 'Enter') sendBtn.click();
      });
    }
  })();
</script>
