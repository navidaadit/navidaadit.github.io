---
permalink: /research/
layout: single
title: "Research"
author_profile: true
---

<!-- ---------- Page-scoped styles (theme-aware; no global side effects) ---------- -->
<style>
.research-lead{font-size:1.06rem;line-height:1.65;margin:.25rem 0 1.15rem;}
.grid-3{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:14px;margin:.75rem 0 1.2rem;}
.grid-2{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:14px;margin:.75rem 0 1.2rem;}
.card{border:1px solid var(--footer-border,#e5e7eb);border-radius:10px;padding:14px;background:var(--footer-bg,#f8fafc);}
.card h4{margin:.1rem 0 .35rem;font-size:1.02rem;}
.stat-row{display:flex;flex-wrap:wrap;gap:8px;margin:.35rem 0 1.1rem;}
.stat-badge{font-size:.9rem;padding:6px 10px;border-radius:999px;border:1px solid var(--tag-border,#e5e7eb);background:var(--tag-bg,#f3f4f6);color:var(--tag-fg,#111827);white-space:nowrap;}
.pill-list{list-style:none;padding:0;margin:.1rem 0 .9rem 0;display:flex;flex-wrap:wrap;gap:6px 8px;}
.pill-list li{font-size:.9rem;padding:6px 10px;border-radius:999px;border:1px solid var(--tag-border,#e5e7eb);background:var(--tag-bg,#f3f4f6);color:var(--tag-fg,#111827);white-space:nowrap;}
.section-h{margin-top:.6rem;}
.small-note{font-size:.92rem;opacity:.9}

/* Kill “double underline” on acronyms — keep tooltip only */
abbr[title]{text-decoration:none;border:0;cursor:help}

/* Spotlight gallery */
.gallery-3{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:12px;margin:.6rem 0 1.2rem;}
.figure-card{position:relative;overflow:hidden;border-radius:10px;border:1px solid var(--footer-border,#e5e7eb);background:var(--footer-bg,#f8fafc);}
.figure-card img{display:block;width:100%;height:220px;object-fit:cover;}
.figcap{padding:8px 10px;font-size:.92rem;border-top:1px solid var(--footer-border,#e5e7eb);}

/* Dark tweaks */
html[data-theme="dark"] .figure-card,
html.dark .figure-card,
body.dark .figure-card,
:root.theme-dark .figure-card{border-color:#1f2937;background:#0b1220;}
html[data-theme="dark"] .figcap,
html.dark .figcap,
body.dark .figcap,
:root.theme-dark .figcap{border-top-color:#1f2937;}

@media (max-width:980px){.grid-3,.grid-2,.gallery-3{grid-template-columns:1fr;}}
</style>

<div class="research-lead">
I work on <strong>probabilistic computers</strong> built from <abbr title="probabilistic bit (binary stochastic neuron)">p-bits</abbr> and <strong>distributed architectures</strong> for fast <strong>sampling</strong>, <strong>learning</strong>, and <strong>quantum-inspired optimization</strong>. My approach is <strong>full-stack</strong> — device physics → architectures → algorithms — scaling from single <abbr title="Field-Programmable Gate Array">FPGA</abbr> systems to multi-FPGA fabrics targeting <strong>million-node</strong> p-computers.
</div>

## Research areas

<div class="grid-3">
  <div class="card">
    <h4>Distributed probabilistic computing</h4>
    <ul>
      <li>Potts-style partitioning for balanced multi-chip mapping</li>
      <li>Latency-aware links that retain solution quality at scale</li>
      <li>Roadmap to 100k–1M+ p-bits</li>
    </ul>
  </div>
  <div class="card">
    <h4>Probabilistic AI & NQS</h4>
    <ul>
      <li>Hardware-aware Deep Boltzmann Machines (DBMs): compact, trainable, generative</li>
      <li>Contrastive-divergence at extreme sweep counts</li>
      <li>Neural Quantum States (NQS) for quantum / scientific data</li>
    </ul>
  </div>
  <div class="card">
    <h4>Quantum-inspired optimization & sampling</h4>
    <ul>
      <li>All-to-all behavior on sparse, massively parallel fabrics</li>
      <li>Higher-order couplings to improve prefactors</li>
      <li>APT, SQA, and non-local MC for hard instances</li>
    </ul>
  </div>
</div>

## Full-stack focus

<div class="grid-3">
  <div class="card">
    <h4>Device / physical layer</h4>
    <ul>
      <li>Binary stochastic neurons: <strong>p-bits</strong></li>
      <li>CMOS today; path to <abbr title="stochastic Magnetic Tunnel Junctions">sMTJs</abbr> for density & energy</li>
      <li>Physics matched to computation: MC / MCMC</li>
    </ul>
  </div>
  <div class="card">
    <h4>Architecture</h4>
    <ul>
      <li><em>Sparse</em> Ising machines with multiplexed <em>all-to-all</em> behavior</li>
      <li>Higher-order interactions (e.g., XORSAT)</li>
      <li>Balanced partitioning for multi-FPGA; delay-tolerant links</li>
      <li>Graph-colored (chromatic) massively parallel Gibbs updates</li>
    </ul>
  </div>
  <div class="card">
    <h4>Algorithms</h4>
    <ul>
      <li>Scalable Gibbs; energy / free-energy diagnostics</li>
      <li>Parallel Tempering (PT) / Adaptive PT (APT)</li>
      <li>Isoenergetic Cluster Moves (ICM)</li>
      <li>Simulated Quantum Annealing (SQA) on heterogeneous fabric</li>
      <li>Deep Boltzmann Machines (DBMs), Energy-Based Models (EBMs)</li>
      <li>Neural Quantum States (NQS) sampling & training</li>
    </ul>
  </div>
</div>

## Key figures of merit

<div class="stat-row">
  <span class="stat-badge">Linear flips/s vs. system size</span>
  <span class="stat-badge">50–64B flips/s (measured)</span>
  <span class="stat-badge">Up to 6 orders vs. CPU Gibbs</span>
  <span class="stat-badge">5–18× vs. TPU/GPU samplers</span>
  <span class="stat-badge">4,264 p-bits (DBM demo)</span>
  <span class="stat-badge">≈30k parameters (DBM demo)</span>
  <span class="stat-badge">All-to-all + higher-order on sparse IMs</span>
  <span class="stat-badge">Multi-FPGA path to 1M+ nodes</span>
</div>

## Spotlight

<div class="gallery-3">
  <figure class="figure-card">
    <img src="/images/research/sparse-ising.jpg" alt="Sparse Ising machine on FPGA">
    <figcaption class="figcap">Sparse Ising machine on FPGA — <em>Nature Electronics</em> (2022)</figcaption>
  </figure>
  <figure class="figure-card">
    <img src="/images/research/dbm-hardware.jpg" alt="Hardware-trained deep Boltzmann machines / NQS">
    <figcaption class="figcap">Hardware-trained DBMs / NQS — <em>Nature Electronics</em> (2024)</figcaption>
  </figure>
  <figure class="figure-card">
    <img src="/images/research/all-to-all.jpg" alt="All-to-all & higher-order Ising machines">
    <figcaption class="figcap">All-to-all & higher-order IMs — <em>Nature Communications</em> (2024)</figcaption>
  </figure>
</div>

<!--
Place three images at:
- /images/research/sparse-ising.jpg
- /images/research/dbm-hardware.jpg
- /images/research/all-to-all.jpg
Aim for ~1200×700px each (landscape), JPG/WEBP.
-->

## Methods I use

<ul class="pill-list">
  <li>Massively parallel (graph-colored) Gibbs</li>
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
