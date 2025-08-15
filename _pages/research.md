---
permalink: /research/
layout: single
title: "Research"
author_profile: true
---

<!-- ---------- Page-scoped styles (theme-aware; no global side effects) ---------- -->
<style>
:root{
  /* fallbacks if your global vars are absent */
  --rail: 14px;
  --card-bg: var(--footer-bg, #f8fafc);
  --card-brd: var(--footer-border, #e5e7eb);
  --pill-bg: var(--tag-bg, #f3f4f6);
  --pill-brd: var(--tag-border, #e5e7eb);
  --pill-fg: var(--tag-fg, #111827);
}

.research-lead{
  font-size:1.06rem;line-height:1.65;margin:.15rem 0 1.1rem;
}

/* KPI row */
.kpi-grid{
  display:grid;grid-template-columns:repeat(3,minmax(0,1fr));
  gap:var(--rail);margin:.5rem 0 1.1rem;
}
.kpi{
  background:var(--card-bg);border:1px solid var(--card-brd);
  border-radius:12px;padding:14px 16px;
}
.kpi h3{margin:0;font-size:1.55rem;letter-spacing:.2px;}
.kpi p{margin:.35rem 0 0 0;font-size:.93rem;opacity:.9}

/* Section cards */
.grid-3{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:var(--rail);margin:.7rem 0 1.2rem}
.card{
  border:1px solid var(--card-brd);border-radius:12px;background:var(--card-bg);
  padding:14px 16px;
}
.card h4{margin:.1rem 0 .4rem;font-size:1.02rem}
.card ul{margin:.1rem 0 .2rem .95rem}

/* Pills / methods */
.pill-list{list-style:none;padding:0;margin:.15rem 0 .9rem;display:flex;flex-wrap:wrap;gap:6px 8px}
.pill-list li{
  font-size:.9rem;line-height:1;padding:7px 11px;border-radius:999px;
  border:1px solid var(--pill-brd);background:var(--pill-bg);color:var(--pill-fg);white-space:nowrap
}

/* Kill default dotted underline on <abbr> but keep tooltip */
abbr[title]{text-decoration:none;border:0;cursor:help}

/* Spotlight gallery (true 16:9, no crop) */
.gallery-3{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:12px;margin:.55rem 0 1.15rem}
.figure-card{position:relative;overflow:hidden;border-radius:12px;border:1px solid var(--card-brd);background:var(--card-bg)}
.figure-card img{
  width:100% !important;height:auto !important;aspect-ratio:16/9 !important;
  object-fit:contain !important;background:transparent !important;display:block
}
.figcap{padding:9px 12px;font-size:.93rem;border-top:1px solid var(--card-brd)}

/* Small note */
.small-note{font-size:.92rem;opacity:.9}

/* Responsive */
@media (max-width:980px){
  .kpi-grid,.grid-3,.gallery-3{grid-template-columns:1fr}
}
</style>

<div class="research-lead">
I work on <strong>probabilistic computers</strong> built from <abbr title="probabilistic bit (binary stochastic neuron)">p-bits</abbr> and <strong>distributed architectures</strong> for fast <strong>sampling</strong>, <strong>learning</strong>, and <strong>quantum-inspired optimization</strong>. The approach is <strong>full-stack</strong> — device physics → architectures → algorithms — scaling from single <abbr title="Field-Programmable Gate Array">FPGA</abbr> systems to multi-FPGA <strong>asynchronous</strong> fabrics targeting <strong>million-node</strong> p-computers.
</div>

<div class="kpi-grid">
  <div class="kpi">
    <h3>50–64B flips/s</h3>
    <p>Measured probabilistic updates on hardware</p>
  </div>
  <div class="kpi">
    <h3>6×10<sup>5</sup>–10<sup>6</sup> scale</h3>
    <p>Roadmap to million-node p-computers</p>
  </div>
  <div class="kpi">
    <h3>5–18× faster</h3>
    <p>Vs. tuned TPU/GPU samplers (task-dependent)</p>
  </div>
</div>

## Research areas

<div class="grid-3">
  <div class="card">
    <h4>Distributed probabilistic computing</h4>
    <ul>
      <li>Probabilistic Potts partitioning for balanced multi-chip mapping</li>
      <li>Latency-aware asynchronous links that retain quality at scale</li>
      <li>Roadmap to 100k–1M+ <abbr title="probabilistic bits">p-bits</abbr></li>
    </ul>
  </div>
  <div class="card">
    <h4>Probabilistic GenAI & quantum simulation</h4>
    <ul>
      <li>Hardware-aware Deep Boltzmann Machines (DBMs)</li>
      <li>Contrastive divergence at extreme sweep counts</li>
      <li>Neural Quantum States (NQS) for quantum/scientific data</li>
    </ul>
  </div>
  <div class="card">
    <h4>Quantum-inspired optimization & sampling</h4>
    <ul>
      <li>All-to-all behavior on sparse, massively parallel fabrics</li>
      <li>Higher-order couplers (e.g., XORSAT) to improve prefactors</li>
      <li>APT, SQA, and non-local MC for hard instances</li>
    </ul>
  </div>
</div>

## Full-stack focus

<div class="grid-3">
  <div class="card">
    <h4>Device / physical layer</h4>
    <ul>
      <li>Asynchronous binary stochastic neurons: <strong>p-bits</strong></li>
      <li>CMOS today → <abbr title="stochastic Magnetic Tunnel Junctions">sMTJs</abbr> next</li>
      <li>Physics ↔ computation (MC/MCMC)</li>
      <li>Quality metrics: energy & free-energy</li>
    </ul>
  </div>
  <div class="card">
    <h4>Architecture</h4>
    <ul>
      <li>Sparse Ising machines with multiplexed all-to-all</li>
      <li>Higher-order interactions; balanced partitioning</li>
      <li>Latency-aware links across multi-FPGA fabrics</li>
      <li>Chromatic, massively parallel Gibbs</li>
    </ul>
  </div>
  <div class="card">
    <h4>Algorithms</h4>
    <ul>
      <li>Simulated Annealing (SA); Parallel Tempering (PT/APT)</li>
      <li>Isoenergetic Cluster Moves (ICM); non-equilibrium MC</li>
      <li>Simulated Quantum Annealing (SQA)</li>
      <li>DBM/EBM training; NQS sampling</li>
    </ul>
  </div>
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

## Methods I use 

<ul class="pill-list">
  <li>Graph-colored (massively parallel) Gibbs</li>
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
