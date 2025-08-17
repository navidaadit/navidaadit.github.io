---
permalink: /research/
layout: single
title: "Research"
author_profile: true
---

<!-- Page-scoped styles (small, theme-aware) -->
<style>
.research-lead{font-size:1.06rem;line-height:1.65;margin:.25rem 0 1.15rem;}
.grid-3{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:14px;margin:.75rem 0 1.2rem;}
.card{border:1px solid var(--footer-border,#e5e7eb);border-radius:10px;padding:14px;background:var(--footer-bg,#f7fafc);}
.card h4{margin:.1rem 0 .35rem;font-size:1.02rem;}
.stat-row{display:flex;flex-wrap:wrap;gap:8px;margin:.35rem 0 1.1rem;}
.stat-badge{font-size:.9rem;padding:6px 10px;border-radius:999px;border:1px solid var(--tag-border,#e5e7eb);background:var(--tag-bg,#f3f4f6);color:var(--tag-fg,#111827);white-space:nowrap;}
.pill-list{list-style:none;padding:0;margin:.1rem 0 .9rem 0;display:flex;flex-wrap:wrap;gap:6px 8px;}
.pill-list li{font-size:.9rem;padding:6px 10px;border-radius:999px;border:1px solid var(--tag-border,#e5e7eb);background:var(--tag-bg,#f3f4f6);color:var(--tag-fg,#111827);white-space:nowrap;}
.small-note{font-size:.92rem;opacity:.9}
abbr[title]{text-decoration:none;border:0;cursor:help}

/* Spotlight grid (2×2). Card/image rules live in global CSS. */
.gallery-2x2{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:12px;margin:.6rem 0 1.2rem;}
@media (max-width:980px){.grid-3,.gallery-2x2{grid-template-columns:1fr;}}

/* ===== HARD OVERRIDE: center ALL captions inside Spotlight cards =====
   Beats global "left !important" by using higher specificity + !important
   and flex centering (works even if text-align is forced elsewhere). */
.layout--single .page__content .gallery-2x2 .figure-card figcaption,
.layout--single .page__content .gallery-2x2 .figure-card .figcap{
  display:flex !important;
  justify-content:center !important;
  text-align:center !important;
  margin-top:6px;
  font-size:.9rem;
  line-height:1.35;
  color:var(--footer-fg,#475569);
}
.layout--single .page__content .gallery-2x2 .figure-card figcaption *,
.layout--single .page__content .gallery-2x2 .figure-card .figcap *{
  text-align:inherit !important; /* inherit the centered alignment */
}
</style>

<div class="research-lead">
I build <strong>CMOS/FPGA systems</strong> for <strong>probabilistic computing</strong> with <abbr title="probabilistic bit (binary stochastic neuron)">p-bits</abbr> (<strong>Ising/Boltzmann machines</strong>) and <strong>distributed architectures</strong> for fast <strong>sampling</strong>, <strong>learning</strong>, and <strong>quantum-inspired optimization</strong>. My approach is <strong>full-stack</strong> — device physics → architectures → algorithms — advancing from single <abbr title="Field-Programmable Gate Array">FPGA</abbr> prototypes to multi-FPGA <strong>asynchronous</strong> fabrics targeting <strong>million-node</strong> p-computers.
</div>

## Research areas

<div class="grid-3">
  <div class="card">
    <h4>Distributed probabilistic computing</h4>
    <ul>
      <li>Balanced multi-chip mapping via probabilistic Potts partitioning</li>
      <li>Asynchronous, latency-tolerant links that preserve solution quality</li>
      <li>Roadmap and measurements toward 100k–1M+ p-bits</li>
    </ul>
  </div>
  <div class="card">
    <h4>Probabilistic Generative AI & ML</h4>
    <ul>
      <li>Hardware-aware Deep Boltzmann Machines (DBMs) and EBMs</li>
      <li>Contrastive-divergence at extreme sweep counts</li>
      <li>Neural Quantum States (NQS) for quantum & scientific data</li>
    </ul>
  </div>
  <div class="card">
    <h4>Quantum-inspired optimization & sampling</h4>
    <ul>
      <li>Sparse fabrics that emulate dense couplings efficiently</li>
      <li>Higher-order couplers to improve prefactors and scaling</li>
      <li>APT, SQA, and non-local MC for hard instances</li>
    </ul>
  </div>
</div>

## Full-stack focus

<div class="grid-3">
  <div class="card">
    <h4>Device / physical layer</h4>
    <ul>
      <li>Physics-inspired <strong>p-bits</strong> (CMOS today; sMTJs next)</li>
      <li>Monte-Carlo-faithful device models and noise tuning</li>
      <li>Quality tracked by energy / free-energy metrics</li>
      <li>Tight device-to-architecture co-design loops</li>
    </ul>
  </div>
  <div class="card">
    <h4>Architecture</h4>
    <ul>
      <li>Sparse IMs with multiplexed dense interactions</li>
      <li>Higher-order interactions (e.g., XORSAT) realized efficiently</li>
      <li>Balanced partitioning & async, latency-tolerant links</li>
      <li>Chromatic, massively parallel Gibbs updates</li>
    </ul>
  </div>
  <div class="card">
    <h4>Algorithms</h4>
    <ul>
      <li>SA / PT with non-local moves (ICM) at scale</li>
      <li>Simulated Quantum Annealing (SQA)</li>
      <li>DBM/EBM training and NQS sampling</li>
      <li>Large-sweep, hardware-aware learning loops</li>
    </ul>
  </div>
</div>

## Key figures of merit

<div class="stat-row">
  <span class="stat-badge">1500B flips/s (measured)</span>
  <span class="stat-badge">Up to 6 orders vs. CPU Gibbs</span>
  <span class="stat-badge">≈100× vs. GPU/TPU (flips/s &amp; energy)</span>
  <span class="stat-badge">6-FPGA UCSB: ~50k p-bits (async links)</span>
  <span class="stat-badge">Synthesized 1M p-bits on 18× VP1902 (Siemens)</span>
  <span class="stat-badge">4,264 p-bits / ≈30k params (DBM)</span>
  <span class="stat-badge">Multi-FPGA path to 1M+ nodes</span>
</div>

## Spotlight

<div class="gallery-2x2">
  <figure class="figure-card">
    <img src="/images/research/sparse-ising.jpeg" alt="Sparse Ising machine on FPGA">
    <figcaption class="figcap">Sparse Ising machine — <em>Nature Electronics</em> (2022)</figcaption>
  </figure>

  <figure class="figure-card">
    <img src="/images/research/dbm-hardware.jpeg" alt="Hardware-trained deep Boltzmann machines">
    <figcaption class="figcap">Hardware-trained DBMs — <em>Nature Electronics</em> (2024)</figcaption>
  </figure>

  <figure class="figure-card">
    <img src="/images/research/all-to-all.jpeg" alt="Higher-order Ising machines and dense behavior">
    <figcaption class="figcap">Higher-order IMs &amp; all-to-all approach — <em>Nature Communications</em> (2024)</figcaption>
  </figure>

  <!-- Rack photo: make it fill the card (no bottom whitespace) -->
  <figure class="figure-card fill">
    <img src="/images/research/5-fpga-setup.jpeg" alt="UCSB multi-FPGA p-computer (rack)">
    <figcaption class="figcap">UCSB multi-FPGA p-computer (~50k p-bits) — lab setup</figcaption>
  </figure>
</div>

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
  <li>NQS sampling &amp; training</li>
</ul>

## Current directions
- <strong>Million-node p-computers:</strong> partitioning and interconnects that preserve solution quality at extreme scale.  
- <strong>Probabilistic AI &amp; NQS at scale:</strong> compact, hardware-efficient learning for scientific/quantum data.  
- <strong>Heterogeneous p-computers:</strong> CMOS + sMTJs to keep improving flips/J and density.

<div class="small-note">
Full publication list: <a href="/publications/">Publications</a>
</div>
