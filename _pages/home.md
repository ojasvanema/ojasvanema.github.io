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
    position: relative;
    min-height: 85vh;
    display: flex;
    align-items: center;
    overflow: hidden;
  }

  .hero-circuit-canvas {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    z-index: 0;
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
    color: #ffffff !important;
    background-color: var(--global-theme-color);
    border: 1px solid var(--global-theme-color);
    border-radius: 6px;
    text-decoration: none !important;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12);
    transition: all 0.2s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .btn-action-primary span {
    color: #ffffff !important;
  }

  .btn-action-primary:hover {
    background-color: #21867a;
    border-color: #21867a;
    color: #ffffff !important;
    box-shadow: 0 2px 8px rgba(42, 157, 143, 0.3);
  }

  .btn-action-primary:hover span {
    color: #ffffff !important;
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

  .btn-action-secondary span {
    color: var(--global-text-color) !important;
  }

  .btn-action-secondary:hover {
    border-color: var(--global-text-color);
    color: var(--global-text-color) !important;
    background-color: rgba(125, 125, 125, 0.08);
  }

  .btn-action-secondary:hover span {
    color: var(--global-text-color) !important;
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
  <!-- Interactive Mechanistic Circuit Canvas -->
  <canvas id="circuit-canvas" class="hero-circuit-canvas"></canvas>

  <div class="row align-items-center w-100" style="position: relative; z-index: 1;">
    
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
          Research Intern at <a href="https://c-d-s.github.io/" target="_blank" style="color: inherit; text-decoration: underline; text-decoration-color: var(--global-theme-color); white-space: nowrap;">Yale University</a><br>
          Undergraduate Researcher at <a href="https://psquare-lab.github.io/" target="_blank" style="color: inherit; text-decoration: underline; text-decoration-color: var(--global-theme-color); white-space: nowrap;">P-Square Lab</a>, IIT Roorkee
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

<script>
  (function() {
    const canvas = document.getElementById('circuit-canvas');
    if (!canvas) return;
    const ctx = canvas.getContext('2d');
    const container = canvas.parentElement;

    let width = 0;
    let height = 0;
    const dpr = window.devicePixelRatio || 1;

    function resize() {
      width = container.clientWidth;
      height = container.clientHeight;
      canvas.width = width * dpr;
      canvas.height = height * dpr;
      canvas.style.width = width + 'px';
      canvas.style.height = height + 'px';
      ctx.scale(dpr, dpr);
    }

    window.addEventListener('resize', resize);
    resize();

    // Circuit & attention node labels representing mechanistic neural internals
    const nodeLabels = [
      'Attn.L2.H1', 'MLP.gate_up', 'Resid.mid', 'QK.route',
      'Attn.L4.H3', 'MLP.down', 'Causal.DAG', 'OV.circuit',
      'Attn.L1.H0', 'Bilinear.proj', 'Kernel.latent', 'Attn.L6.H4',
      'Disentangle.W', 'MLP.act', 'Unlearn.ortho', 'Score.grad'
    ];

    const nodeCount = Math.min(34, Math.max(20, Math.floor((width * height) / 20000)));
    const nodes = [];

    for (let i = 0; i < nodeCount; i++) {
      const isAttn = Math.random() > 0.45;
      nodes.push({
        x: Math.random() * width,
        y: Math.random() * height,
        vx: (Math.random() - 0.5) * 0.4,
        vy: (Math.random() - 0.5) * 0.4,
        type: isAttn ? 'attn' : 'mlp',
        radius: isAttn ? 3.2 : 2.8,
        label: nodeLabels[i % nodeLabels.length],
        pulse: Math.random() * Math.PI * 2,
        pulseSpeed: 0.018 + Math.random() * 0.02
      });
    }

    // Mouse probe tracking
    const mouse = { x: -1000, y: -1000, active: false };

    container.addEventListener('mousemove', function(e) {
      const rect = container.getBoundingClientRect();
      mouse.x = e.clientX - rect.left;
      mouse.y = e.clientY - rect.top;
      mouse.active = true;
    });

    container.addEventListener('mouseleave', function() {
      mouse.active = false;
      mouse.x = -1000;
      mouse.y = -1000;
    });

    function isDarkMode() {
      return document.documentElement.getAttribute('data-theme') === 'dark' ||
        (!document.documentElement.getAttribute('data-theme') && window.matchMedia('(prefers-color-scheme: dark)').matches);
    }

    let isVisible = true;
    if ('IntersectionObserver' in window) {
      const observer = new IntersectionObserver(function(entries) {
        isVisible = entries[0].isIntersecting;
      });
      observer.observe(container);
    }

    function render() {
      if (isVisible) {
        ctx.clearRect(0, 0, width, height);
        const dark = isDarkMode();

        // Elegant, restrained colors:
        // Teal (#2a9d8f) for Attention heads, Slate-blue (#2a6f97) for MLP gates
        const attnColor = dark ? '42, 157, 143' : '30, 130, 120';
        const mlpColor = dark ? '60, 130, 190' : '42, 111, 151';
        const lineColor = dark ? '148, 163, 184' : '100, 116, 139';

        // 1. Passive subtle circuit traces between nearby nodes
        for (let i = 0; i < nodes.length; i++) {
          const n = nodes[i];
          n.x += n.vx;
          n.y += n.vy;
          n.pulse += n.pulseSpeed;

          if (n.x < 12) { n.x = 12; n.vx *= -1; }
          if (n.x > width - 12) { n.x = width - 12; n.vx *= -1; }
          if (n.y < 12) { n.y = 12; n.vy *= -1; }
          if (n.y > height - 12) { n.y = height - 12; n.vy *= -1; }

          for (let j = i + 1; j < nodes.length; j++) {
            const n2 = nodes[j];
            const dx = n.x - n2.x;
            const dy = n.y - n2.y;
            const dist = Math.sqrt(dx * dx + dy * dy);

            if (dist < 115) {
              const alpha = (1 - dist / 115) * (dark ? 0.08 : 0.05);
              ctx.strokeStyle = `rgba(${lineColor}, ${alpha})`;
              ctx.lineWidth = 0.75;
              ctx.beginPath();
              ctx.moveTo(n.x, n.y);
              ctx.lineTo(n2.x, n2.y);
              ctx.stroke();
            }
          }
        }

        // 2. Interactive probe: active connection traces to cursor
        if (mouse.active) {
          for (let i = 0; i < nodes.length; i++) {
            const n = nodes[i];
            const dx = n.x - mouse.x;
            const dy = n.y - mouse.y;
            const dist = Math.sqrt(dx * dx + dy * dy);

            if (dist < 145) {
              const probeAlpha = (1 - dist / 145) * (dark ? 0.32 : 0.25);
              ctx.strokeStyle = `rgba(${attnColor}, ${probeAlpha})`;
              ctx.lineWidth = 0.9;
              ctx.setLineDash([3, 4]); // delicate dashed line trace
              ctx.beginPath();
              ctx.moveTo(mouse.x, mouse.y);
              ctx.lineTo(n.x, n.y);
              ctx.stroke();
              ctx.setLineDash([]);

              // Display technical node label on cursor approach
              const textAlpha = (1 - dist / 145) * 0.7;
              ctx.font = '9px SFMono-Regular, Menlo, Monaco, Consolas, monospace';
              ctx.fillStyle = `rgba(${dark ? '203, 213, 225' : '71, 85, 105'}, ${textAlpha})`;
              ctx.fillText(n.label, n.x + 8, n.y - 4);
            }
          }
        }

        // 3. Draw nodes
        for (let i = 0; i < nodes.length; i++) {
          const n = nodes[i];
          const pulse = Math.sin(n.pulse) * 0.12;
          const baseAlpha = dark ? (0.35 + pulse) : (0.28 + pulse);

          if (n.type === 'attn') {
            // Circular Attention node with subtle ring
            ctx.fillStyle = `rgba(${attnColor}, ${baseAlpha})`;
            ctx.beginPath();
            ctx.arc(n.x, n.y, n.radius, 0, Math.PI * 2);
            ctx.fill();

            ctx.strokeStyle = `rgba(${attnColor}, ${baseAlpha * 0.45})`;
            ctx.lineWidth = 0.6;
            ctx.beginPath();
            ctx.arc(n.x, n.y, n.radius + 2.5, 0, Math.PI * 2);
            ctx.stroke();
          } else {
            // Diamond MLP gate node
            ctx.fillStyle = `rgba(${mlpColor}, ${baseAlpha})`;
            const r = n.radius;
            ctx.beginPath();
            ctx.moveTo(n.x, n.y - r);
            ctx.lineTo(n.x + r, n.y);
            ctx.lineTo(n.x, n.y + r);
            ctx.lineTo(n.x - r, n.y);
            ctx.closePath();
            ctx.fill();
          }
        }
      }

      requestAnimationFrame(render);
    }

    requestAnimationFrame(render);
  })();
</script>
