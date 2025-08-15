---
permalink: /research/
layout: single
title: "Research"
author_profile: true
---

<!-- ---------- Page-scoped lightweight styles (theme-aware; no global side effects) ---------- -->
<style>
.research-lead{font-size:1.06rem;line-height:1.65;margin:.25rem 0 1.25rem;}
.grid-3{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:14px;margin:.75rem 0 1.25rem;}
.grid-2{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:14px;margin:.75rem 0 1.25rem;}
.card{border:1px solid var(--footer-border,#e5e7eb);border-radius:10px;padding:14px 14px 12px;background:var(--footer-bg,#f8fafc);}
.card h4{margin:.1rem 0 .35rem;font-size:1.02rem;}
.stat-row{display:flex;flex-wrap:wrap;gap:8px;margin:.35rem 0 1.1rem;}
.stat-badge{font-size:.9rem;padding:6px 10px;border-radius:999px;border:1px solid var(--tag-border,#e5e7eb);background:var(--tag-bg,#f3f4f6);color:var(--tag-fg,#111827);white-space:nowrap;}
.pill-list{list-style:none;padding:0;margin:.1rem 0 .9rem 0;display:flex;flex-wrap:wrap;gap:6px 8px;}
.pill-list li{font-size:.9rem;padding:6px 10px;border-radius:999px;border:1px solid var(--tag-border,#e5e7eb);background:var(--tag-bg,#f3f4f6);color:var(--tag-fg,#111827);white-space:nowrap;}
.section-h{margin-top:.6rem;}
.small-note{font-size:.92rem;opacity:.9}
abbr[title]{text-decoration:underline dotted;cursor:help}

/* Mobile */
@media (max-width:980px){
  .grid-3{grid-template-columns:1fr;}
  .grid-2{grid-template-columns:1fr;}
}
</style>

<div class="research-lead">
I design <strong>probabilistic computers</strong> based on <abbr title="probabilistic bit">p-bits</abbr> and <strong>distributed architectures</strong> for fast <strong>sampling</strong>, <strong>learning</strong>, and <strong>quantum-inspired optimization</strong> — scaling from a single <abbr title="Field-Programmable Gate Array">FPGA</abbr> to multi-FPGA fabrics, with a path toward <strong>million-node</strong> systems. A consistent <strong>full-stack</strong> approach ties together device physics, architectures, and algorithms.
</div>

## Full-stack perspective

<div class="grid-3">
  <div class="card">
    <h4>Device / Physical layer</h4>
    <ul>
      <li><abbr title="probabilistic bit">p-bits</abbr> as binary stochastic neurons</li>
      <li>CMOS realizations; roadmap to <abbr title="stochastic Magnetic Tunnel Junction">sMTJs</abbr> for density & energy</li>
      <li>Physics matched to computation (<abbr title="Monte Carlo">MC</abbr> / <abbr title="Markov chain Monte Carlo">MCMC</abbr> sampling)</li>
    </ul>
  </div>
  <div class="card">
    <h4>Architecture</h4>
    <ul>
      <li><em>Sparse</em> fabrics with <em>multiplexed all-to-all</em> behavior</li>
      <li>Higher-order interactions (e.g., XORSAT)</li>
      <li>Balanced partitioning for multi-FPGA; delay-tolerant links</li>
      <li>Chromatic (<abbr title="graph-colored parallel Gibbs updates">graph-colored</abbr>) parallel updates</li>
    </ul>
  </div>
  <div class="card">
    <h4>Algorithms</h4>
    <ul>
      <li>Gibbs sampling at scale; energy/free-energy diagnostics</li>
      <li><abbr title="Parallel Tempering">PT</abbr> / <abbr title="Adaptive Parallel Tempering">APT</abbr></li>
      <li>Non-local <abbr title="Monte Carlo">MC</abbr> (ICM / Houdayer-type moves)</li>
      <li><abbr title="Simulated Quantum Annealing">SQA</abbr> on heterogeneous fabric</li>
      <li><abbr title="Neural Quantum States">NQS</abbr> & <abbr title="Energy-Based Models">EBM</abbr> learning on hardware</li>
    </ul>
  </div>
</div>

## Focus areas

<div class="grid-3">
  <div class="card">
    <h4>Distributed probabilistic computing</h4>
    <ul>
      <li>Potts-style partitioning for balanced multi-chip mapping</li>
      <li>Latency-aware links with quality retention at scale</li>
      <li>Control & telemetry toward 100k–1M+ p-bits</li>
    </ul>
  </div>
  <div class="card">
    <h4>Probabilistic AI & NQS</h4>
    <ul>
      <li>Hardware-aware Deep Boltzmann Machines (<abbr title="Deep Boltzmann Machine">DBM</abbr>)</li>
      <li>Compact parameterization with generative capability</li>
      <li><abbr title="Neural Quantum States">NQS</abbr>: sampling & training on p-computers</li>
    </ul>
  </div>
  <div class="card">
    <h4>Quantum-inspired optimization & sampling</h4>
    <ul>
      <li>All-to-all behavior on sparse, massively parallel fabrics</li>
      <li>Higher-order couplings to improve prefactors</li>
      <li><abbr title="Adaptive Parallel Tempering">APT</abbr>, <abbr title="Simulated Quantum Annealing">SQA</abbr>, and non-local MC for hard instances</li>
    </ul>
  </div>
</div>

## Impact snapshots

<div class="stat-row">
  <span class="stat-badge">Linear flips/s with system size</span>
  <span class="stat-badge">50–64B flips/s (measured)</span>
  <span class="stat-badge">Up to 6 orders vs CPU Gibbs</span>
  <span class="stat-badge">5–18× vs TPU/GPU samplers</span>
  <span class="stat-badge">4,264 p-bits (DBMs)</span>
  <span class="stat-badge">All-to-all + higher-order on sparse IMs</span>
  <span class="stat-badge">Multi-FPGA path to 1M+ nodes</span>
</div>

## Representative results

<div class="grid-3">
  <div class="card">
    <h4>Massively parallel sparse Ising machines</h4>
    <div>Flips/s scale linearly; strong gains vs CPU/TPU/GPU; robust ground states even with faster (inexact) clocks. <em>Nature Electronics (2022)</em></div>
  </div>
  <div class="card">
    <h4>DBMs & NQS on hardware</h4>
    <div>Hardware-aware DBMs reach software-level accuracy with far fewer parameters; sustained 50–64B flips/s; CD-<em>n</em> up to 10M. Extends naturally to <strong>NQS</strong> workflows. <em>Nature Electronics (2024)</em></div>
  </div>
  <div class="card">
    <h4>All-to-all & higher-order on sparse fabrics</h4>
    <div>Multiplexed all-to-all while preserving parallel Gibbs; higher-order interactions improve prefactors on XORSAT. <em>Nature Communications (2024)</em></div>
  </div>
</div>

## Algorithm toolbox (what I run in practice)
<ul class="pill-list">
  <li>Chromatic Gibbs (<abbr title="graph-colored parallel updates">graph-colored</abbr>)</li>
  <li><abbr title="Adaptive Parallel Tempering">APT</abbr></li>
  <li><abbr title="Simulated Quantum Annealing">SQA</abbr></li>
  <li><abbr title="Ising-Cluster Moves (Houdayer)">ICM</abbr> non-local moves</li>
  <li>Non-equilibrium <abbr title="Monte Carlo">MC</abbr></li>
  <li>All-to-all emulation (multiplexed)</li>
  <li>Higher-order couplings</li>
  <li>Energy / free-energy diagnostics</li>
  <li><abbr title="Deep Boltzmann Machine">DBM</abbr> / <abbr title="Energy-Based Model">EBM</abbr> training (hardware-aware)</li>
  <li><abbr title="Neural Quantum States">NQS</abbr> sampling & training</li>
</ul>

## Current directions
- <strong>Million-node p-computers:</strong> partitioning + interconnects that preserve solution quality at extreme scale.  
- <strong>Probabilistic AI & NQS at scale:</strong> compact, hardware-efficient learning for scientific/quantum data.  
- <strong>Heterogeneous p-computers:</strong> CMOS + <abbr title="stochastic Magnetic Tunnel Junction">sMTJs</abbr> to keep improving flips/J and density.

<div class="small-note">
Full publication list: <a href="/publications/">/publications/</a>
</div>

---

### Acronym glossary (at a glance)
- **p-bit** — probabilistic bit (binary stochastic neuron realized in hardware)  
- **IM** — Ising machine  
- **FPGA** — Field-Programmable Gate Array  
- **MC** — Monte Carlo  
- **MCMC** — Markov chain Monte Carlo  
- **PT** — Parallel Tempering  
- **APT** — Adaptive Parallel Tempering  
- **SQA** — Simulated Quantum Annealing  
- **ICM** — Ising-Cluster Moves (Houdayer-type non-local updates)  
- **DBM** — Deep Boltzmann Machine  
- **EBM** — Energy-Based Model  
- **NQS** — Neural Quantum States  
- **sMTJ** — stochastic Magnetic Tunnel Junction  
- **XORSAT** — exclusive-OR satisfiability (higher-order constraint family)
