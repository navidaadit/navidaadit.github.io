---
permalink: /research/
layout: single
title: "Research"
author_profile: true
---

<!-- ---------- Page-scoped styles (theme-aware; content unchanged) ---------- -->
<style>
:root{
  --g:14px;                 /* grid gap */
  --radius:12px;            /* card radius */
  --shadow:0 6px 20px rgba(0,0,0,.06);
  --card-bg:var(--footer-bg,#f8fafc);
  --card-br:var(--footer-border,#e5e7eb);
  --pill-bg:var(--tag-bg,#f3f4f6);
  --pill-br:var(--tag-border,#e5e7eb);
  --pill-fg:var(--tag-fg,#111827);
  --media-bg:rgba(0,0,0,.04); /* shows behind letterboxed images */
}

/* lead paragraph */
.research-lead{font-size:1.06rem;line-height:1.65;margin:.25rem 0 1.15rem}

/* responsive 3-up grid (collapses gracefully) */
.grid-3{
  display:grid;
  grid-template-columns:repeat(3,minmax(0,1fr));
  gap:var(--g);
  margin:.75rem 0 1.2rem;
}
.grid-2{
  display:grid;
  grid-template-columns:repeat(2,minmax(0,1fr));
  gap:var(--g);
  margin:.75rem 0 1.2rem;
}

/* modern card */
.card{
  border:1px solid var(--card-br);
  border-radius:var(--radius);
  padding:16px 16px 14px;
  background:var(--card-bg);
  box-shadow:var(--shadow);
  transition:transform .15s ease, box-shadow .15s ease;
}
.card:hover{ transform:translateY(-2px); box-shadow:0 10px 26px rgba(0,0,0,.10) }
.card h4{ margin:.1rem 0 .45rem; font-size:1.02rem }

/* stat badges */
.stat-row{ display:flex; flex-wrap:wrap; gap:8px; margin:.35rem 0 1.1rem }
.stat-badge{
  font-size:.9rem; padding:6px 10px; border-radius:999px;
  border:1px solid var(--pill-br); background:var(--pill-bg); color:var(--pill-fg);
  white-space:nowrap
}

/* method pills */
.pill-list{ list-style:none; padding:0; margin:.1rem 0 .9rem 0; display:flex; flex-wrap:wrap; gap:6px 8px }
.pill-list li{
  font-size:.9rem; padding:6px 10px; border-radius:999px; white-space:nowrap;
  border:1px solid var(--pill-br); background:var(--pill-bg); color:var(--pill-fg)
}

/* kill browser underline on acronyms; keep tooltip */
abbr[title]{ text-decoration:none; border:0; cursor:help }

/* ---------- Spotlight gallery: NO CROPPING (keeps 16:9 fully) ---------- */
.gallery-3{
  display:grid;
  grid-template-columns:repeat(3,minmax(0,1fr));
  gap:12px; margin:.6rem 0 1.2rem
}
.figure-card{
  position:relative; overflow:hidden; border-radius:var(--radius);
  border:1px solid var(--card-br); background:var(--card-bg); box-shadow:var(--shadow)
}

/* Show full image without cropping. Aspect-ratio ensures consistent height. */
.figure-card img{
  display:block; width:100%; height:auto;
  aspect-ratio:16/9;         /* consistent frame */
  object-fit:contain;         /* NO CROP */
  background:var(--media-bg); /* subtle letterbox fill */
}
.figcap{
  padding:10px 12px; font-size:.92rem;
  border-top:1px solid var(--card-br)
}

/* dark tweaks for borders/backgrounds */
html[data-theme="dark"] .figure-card,
html.dark .figure-card,
body.dark .figure-card,
:root.theme-dark .figure-card{ border-color:#1f2937; background:#0b1220 }
html[data-theme="dark"] .figcap,
html.dark .figcap,
body.dark .figcap,
:root.theme-dark .figcap{ border-top-color:#1f2937 }
:root.theme-dark{ --media-bg:rgba(255,255,255,.06) }

/* responsive collapse */
@media (max-width:980px){ .grid-3,.grid-2,.gallery-3{ grid-template-columns:1fr } }
</style>

<div class="research-lead">
I work on <strong>probabilistic computers</strong> built from <abbr title="probabilistic bit (binary stochastic neuron)">p-bits</abbr> and <strong>distributed architectures</strong> for fast <strong>sampling</strong>, <strong>learning</strong>, and <strong>quantum-inspired optimization</strong>. My approach is <strong>full-stack</strong> — device physics → architectures → algorithms — scaling from single <abbr title="Field-Programmable Gate Array">FPGA</abbr> systems to multi-FPGA <strong>asynchronous</strong> fabrics targeting <strong>million-node</strong> p-computers.
</div>

## Research areas

<div class="grid-3">
  <div class="card">
    <h4>Distributed probabilistic computing</h4>
    <ul>
      <li>Probabilistic Potts partitioning for balanced multi-chip mapping</li>
      <li>Latency-aware asynchronous links that retain solution quality at scale</li>
      <li>Roadmap to 100k–1M+ p-bits</li>
    </ul>
  </div>
  <div class="card">
    <h4>Probabilistic GenAI & Quantum simulation</h4>
    <ul>
      <li>Hardware-aware Deep Boltzmann Machines (DBMs)</li>
      <li>Contrastive-divergence at extreme sweep counts</li>
      <li>Neural Quantum States (NQS) for quantum/science data</li>
    </ul>
  </div>
  <div class="card">
    <h4>Quantum-inspired optimization & sampling</h4>
    <ul>
      <li>All-to-all behavior on sparse, parallel fabrics</li>
      <li>Higher-order couplers to improve prefactors</li>
      <li>APT, SQA, and non-local MC for hard instances</li>
    </ul>
  </div>
</div>

## Full-stack focus

<div class="grid-3">
  <div class="card">
    <h4>Device / physical layer</h4>
    <ul>
      <li>Asynchronous: <strong>p-bits</strong></li>
      <li>CMOS today → <abbr title="stochastic Magnetic Tunnel Junctions">sMTJs</abbr> next</li>
      <li>Physics ↔ computation</li>
      <li>Quality metrics: energy / free-energy</li>
    </ul>
  </div>
  <div class="card">
    <h4>Architecture</h4>
    <ul>
      <li>Sparse IMs with multiplexed all-to-all</li>
      <li>Higher-order interactions (e.g., XORSAT)</li>
      <li>Balanced partitioning, latency-aware asynchronous links</li>
      <li>Chromatic, massively parallel Gibbs</li>
    </ul>
  </div>
  <div class="card">
    <h4>Algorithms</h4>
    <ul>
      <li>Simulated Annealing (SA)/ Parallel Tempering (PT)</li>
      <li>Isoenergetic Cluster Moves (ICM)</li>
      <li>Simulated Quantum Annealing (SQA)</li>
      <li>DBM/EBM training; NQS sampling</li>
    </ul>
  </div>
</div>

## Key figures of merit

<div class="stat-row">
  <span class="stat-badge">Linear flips/s vs. system size</span>
  <span class="stat-badge">1500B flips/s (measured)</span>
  <span class="stat-badge">Up to 6 orders vs. CPU Gibbs</span>
  <span class="stat-badge">5–18× vs. TPU/GPU samplers</span>
  <span class="stat-badge">4,264 p-bits / ≈30k params (DBM)</span>
  <span class="stat-badge">All-to-all + higher-order on sparse IMs</span>
  <span class="stat-badge">Multi-FPGA path to 1M+ nodes</span>
</div>

## Spotlight

<div class="gallery-3">
  <figure class="figure-card">
    <img src="/images/research/sparse-ising.jpeg" alt="Sparse Ising machine on FPGA">
    <figcaption class="figcap">Sparse Ising machine on FPGA — <em>Nature Electronics</em> (2022)</figcaption>
  </figure>
  <figure class="figure-card">
    <img src="/images/research/dbm-hardware.jpeg" alt="Hardware-trained deep Boltzmann machines">
    <figcaption class="figcap">Hardware-trained DBMs — <em>Nature Electronics</em> (2024)</figcaption>
  </figure>
  <figure class="figure-card">
    <img src="/images/research/all-to-all.jpeg" alt="All-to-all & higher-order Ising machines">
    <figcaption class="figcap">All-to-all & higher-order IMs — <em>Nature Communications</em> (2024)</figcaption>
  </figure>
</div>

<!-- Images expected at:
- /images/research/sparse-ising.jpeg
- /images/research/dbm-hardware.jpeg
- /images/research/all-to-all.jpeg
Use 16:9 (e.g., 1280×720 or 1600×900). They’ll be letterboxed, not cropped. -->

## Methods I use

<ul class="pill-list">
  <li>Massively parallel (graph-colored) Gibbs</li>
  <li>Simulated Annealing (SA)</li>
  <li>Adaptive Parallel Tempering (APT)</li>
  <li>Simulated Quantum Annealing (SQA)</li>
  <li>Isoenergetic Cluster Moves (ICM)</li>
  <li>Non-equilibrium Monte Carlo (NMC)</li>
  <li>Higher-order p-bits / couplers</li>
  <li>DBM training (hardware-aware)</li>
  <li>NQS sampling & training</li>
</ul>

## Current directions
- <strong>Million-node p-computers:</strong> partitioning and interconnects that preserve solution quality at extreme scale.  
- <strong>Probabilistic AI & NQS at scale:</strong> compact, hardware-efficient learning for scientific/quantum data.  
- <strong>Heterogeneous p-computers:</strong> CMOS + sMTJs to keep improving flips/J and density.

<div class="small-note">
Full publication list: <a href="/publications/">/publications/</a>
</div>
