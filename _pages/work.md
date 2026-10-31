---
layout: page
title: Work
permalink: /work/
nav: true
nav_order: 2
---

<!-- Achievements Section -->
<h2 class="category">Achievements & Honors</h2>
<div class="achievements-section mb-5">
  <div class="py-3 border-bottom">
    <div class="row">
      <div class="col-md-9">
        <h5 class="font-weight-bold mb-1">Google DeepMind APAC Research Symposium 2026</h5>
        <p class="text-muted mb-0">Selected as a student research delegate.</p>
      </div>
      <div class="col-md-3 text-md-right text-muted">
        <small>2026</small>
      </div>
    </div>
  </div>

  <div class="py-3 border-bottom">
    <div class="row">
      <div class="col-md-9">
        <h5 class="font-weight-bold mb-1">EY Techathon 6.0</h5>
        <p class="text-muted mb-0">Secured a Top-3 finish among 180,000+ participants nationwide.</p>
      </div>
      <div class="col-md-3 text-md-right text-muted">
        <small>2026</small>
      </div>
    </div>
  </div>

  <div class="py-3 border-bottom">
    <div class="row">
      <div class="col-md-9">
        <h5 class="font-weight-bold mb-1">Amazon ML Challenge 2025</h5>
        <p class="text-muted mb-0">Ranked 66th out of 82,789 participants in a national ML competition.</p>
      </div>
      <div class="col-md-3 text-md-right text-muted">
        <small>2025</small>
      </div>
    </div>
  </div>

  <div class="py-3 border-bottom">
    <div class="row">
      <div class="col-md-9">
        <h5 class="font-weight-bold mb-1">STC-UP Hackathon</h5>
        <p class="text-muted mb-0">Ranked Top 11 across India; only undergraduate team competing against industry startups.</p>
      </div>
      <div class="col-md-3 text-md-right text-muted">
        <small>2025</small>
      </div>
    </div>
  </div>
</div>


<!-- Research & Professional Experience Section -->
<h2 class="category mt-5">Research & Professional Experience</h2>
<div class="experience-section mb-5">
  
  <div class="job py-3 border-bottom">
    <div class="row">
      <div class="col-md-9">
        <h4 class="font-weight-bold">Research Intern</h4>
        <h5 class="text-muted">Causal Evidence & Decisions Studio, <a href="https://c-d-s.github.io/" target="_blank">Prof. Harsh Parikh</a> &ndash; Yale University</h5>
      </div>
      <div class="col-md-3 text-md-right text-muted">
        <small>May 2026 &ndash; Jul 2026<br>New Haven, USA</small>
      </div>
    </div>
    <div class="mt-2">
      <ul>
        <li>Formulating a theoretical framework to construct Confidence Sets of Representations.</li>
        <li>Implemented and evaluated multiple causal representation learning algorithms, applying structural relaxations to bound the unidentifiable representation space.</li>
        <li>Overcoming the limitations of purely predictive models by recovering true causal mechanisms, enabling robust counterfactual reasoning and scientific discovery.</li>
      </ul>
    </div>
  </div>

  <div class="job py-3 border-bottom">
    <div class="row">
      <div class="col-md-9">
        <h4 class="font-weight-bold">Undergraduate Research Assistant</h4>
        <h5 class="text-muted"><a href="https://psquare-lab.github.io/" target="_blank">P-Square Lab</a>, Prof. Parikshit Pareek &ndash; IIT Roorkee</h5>
      </div>
      <div class="col-md-3 text-md-right text-muted">
        <small>Sep 2025 &ndash; Present<br>Roorkee, India</small>
      </div>
    </div>
    <div class="mt-2">
      <ul>
        <li>Demonstrated orthogonal task structures induce disentanglement in MLPs, enabling surgical unlearning. <a href="https://arxiv.org/abs/2602.05635" target="_blank">[Read Paper]</a></li>
        <li>Designed amortized inference for zero-shot Gaussian Process kernel discovery from limited data using PFNs.</li>
        <li>Engineered a sparsity-aware latent diffusion model for ultra-sparse jet image synthesis in high-energy physics (CERN). <a href="https://drive.google.com/file/d/1gd-tJp-8napvR_qcfLp3wWk1FNH72SFo/view?usp=drive_link" target="_blank">[Read Paper]</a></li>
      </ul>
    </div>
  </div>

  <div class="job py-3 border-bottom">
    <div class="row">
      <div class="col-md-9">
        <h4 class="font-weight-bold">Research Engineer</h4>
        <h5 class="text-muted"><a href="https://elimentary.com/" target="_blank">Elimentary</a> (YC F26)</h5>
      </div>
      <div class="col-md-3 text-md-right text-muted">
        <small>Nov 2025 &ndash; Jan 2026<br>Bangalore, India</small>
      </div>
    </div>
    <div class="mt-2">
      <ul>
        <li>Built secure, quantized local LLM APIs, achieving granular layer-wise observability.</li>
        <li>Optimized GPU throughput by implementing sequence scheduling for concurrent LLM inference requests.</li>
        <li>Designed a no-code LLM evaluation platform integrated with Langfuse and Grafana for comprehensive monitoring.</li>
      </ul>
    </div>
  </div>

</div>


<!-- Publications Section -->
<h2 class="category mt-5">Publications</h2>
<div class="publications">
{% include selected_papers.liquid %}
</div>

<!-- Terminal-style Toast Notification for BibTeX Copier -->
<div id="terminal-toast" class="terminal-toast" role="status" aria-live="polite">
  <div class="terminal-toast-bar">
    <span class="terminal-dot red"></span>
    <span class="terminal-dot yellow"></span>
    <span class="terminal-dot green"></span>
    <span class="terminal-toast-tag">terminal</span>
  </div>
  <div class="terminal-toast-content">
    <span class="terminal-prompt">$</span>
    <span class="terminal-msg">bibtex copied to clipboard</span>
  </div>
</div>

<style>
  .bibtex-copy-btn {
    transition: all 0.2s ease !important;
  }
  
  .bibtex-copy-btn.copied {
    border-color: var(--global-theme-color) !important;
    color: var(--global-theme-color) !important;
  }

  .terminal-toast {
    position: fixed;
    bottom: 28px;
    right: 28px;
    z-index: 9999;
    min-width: 270px;
    background: rgba(18, 22, 28, 0.94);
    color: #e2e8f0;
    border: 1px solid rgba(42, 157, 143, 0.45);
    border-radius: 8px;
    box-shadow: 0 16px 36px rgba(0, 0, 0, 0.35), 0 0 1px rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(12px);
    -webkit-backdrop-filter: blur(12px);
    font-family: SFMono-Regular, Menlo, Monaco, Consolas, monospace;
    font-size: 0.82rem;
    padding: 8px 14px;
    opacity: 0;
    transform: translateY(16px);
    pointer-events: none;
    transition: opacity 0.25s cubic-bezier(0.16, 1, 0.3, 1), transform 0.25s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .terminal-toast.show {
    opacity: 1;
    transform: translateY(0);
  }

  .terminal-toast-bar {
    display: flex;
    align-items: center;
    gap: 5px;
    margin-bottom: 5px;
    padding-bottom: 4px;
    border-bottom: 1px solid rgba(255, 255, 255, 0.08);
  }

  .terminal-dot {
    width: 7px;
    height: 7px;
    border-radius: 50%;
    display: inline-block;
  }

  .terminal-dot.red { background: #ff5f56; }
  .terminal-dot.yellow { background: #ffbd2e; }
  .terminal-dot.green { background: #27c93f; }

  .terminal-toast-tag {
    font-size: 0.68rem;
    color: #94a3b8;
    margin-left: auto;
    text-transform: uppercase;
    letter-spacing: 0.06em;
  }

  .terminal-toast-content {
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .terminal-prompt {
    color: var(--global-theme-color);
    font-weight: 700;
  }
</style>

<script>
  (function() {
    let toastTimeout = null;
    const toast = document.getElementById('terminal-toast');

    document.addEventListener('click', function(e) {
      const btn = e.target.closest('.bibtex-copy-btn');
      if (!btn) return;
      e.preventDefault();

      const key = btn.getAttribute('data-key');
      const rawEl = document.getElementById('bibtex-raw-' + key);
      if (!rawEl) return;

      const bibtexText = rawEl.textContent.trim();
      navigator.clipboard.writeText(bibtexText).then(function() {
        // Button tactile feedback
        const originalHtml = btn.innerHTML;
        btn.innerHTML = '<i class="fa-solid fa-check mr-1" style="color: var(--global-theme-color);"></i>Copied!';
        btn.classList.add('copied');

        setTimeout(function() {
          btn.innerHTML = originalHtml;
          btn.classList.remove('copied');
        }, 1800);

        // Terminal toast animation
        if (toast) {
          toast.classList.add('show');
          if (toastTimeout) clearTimeout(toastTimeout);
          toastTimeout = setTimeout(function() {
            toast.classList.remove('show');
          }, 2400);
        }
      }).catch(function(err) {
        console.error('Failed to copy bibtex:', err);
      });
    });
  })();
</script>
