---
permalink: /research/
layout: single
title: "Research"
author_profile: true
---

<!-- ---------- Page-scoped lightweight styles ---------- -->
<style>
.research-lead { font-size:1.06rem; line-height:1.65; margin:.25rem 0 1.25rem; }

.card-grid { display:grid; grid-template-columns:repeat(3,minmax(0,1fr)); gap:14px; margin:.75rem 0 1.25rem; }
.card { border:1px solid var(--footer-border, #e5e7eb); border-radius:10px; padding:14px 14px 12px; background:var(--footer-bg, #f8fafc); }
.card h4 { margin:.1rem 0 .35rem; font-size:1.02rem; }

.stat-row { display:flex; flex-wrap:wrap; gap:8px; margin:.35rem 0 1.1rem; }
.stat-badge { font-size:.9rem; padding:6px 10px; border-radius:999px; border:1px solid var(--tag-border, #e5e7eb); background:var(--tag-bg, #f3f4f6); color:var(--tag-fg, #111827); white-space:nowrap; }

.pill-list { list-style:none; padding:0; margin:.1rem 0 .9rem 0; display:flex; flex-wrap:wrap; gap:6px 8px; }
.pill-list li { font-size:.9rem; padding:6px 10px; border-radius:999px; border:1px solid var(--tag-border, #e5e7eb); background:var(--tag-bg, #f3f4f6); color:var(--tag-fg, #111827); white-space:nowrap; }

.section-h { margin-top:.6rem; }

/* Optional thumbnail gallery */
.thumb-grid { display:grid; grid-template-columns:repeat(3,minmax(0,1fr)); gap:10px; margin:.4rem 0 1.2rem; }
.thumb { border:1px solid var(--tag-border, #e5e7eb); border-radius:10px; overflow:hidden; background:var(--footer-bg, #f8fafc); }
.thumb img { display:block; width:100%; height:auto; }
.thumb figcaption { font-size:.9rem; padding:8px 10px; opacity:.9; }

/* Mobile */
@media (max-width:980px){
  .card-grid{ grid-template-columns:1fr; }
  .thumb-grid{ grid-template-columns:1fr; }
}
</style>

<div class="research-lead">
I develop <strong>probabilistic computers (p-computers)</strong> and <strong>distributed architectures</strong> for fast sampling, learning, and hard optimization — from single FPGAs to <strong>multi-FPGA</strong> fabrics, with a roadmap toward <strong>million-node</strong> scale. My work blends statistical physics, machine learning, and quantum-inspired methods.
</div>

### Focus areas
<div class="card-grid">
  <div class="card">
    <h4>Distributed probabilistic computing</h4>
    <ul>
      <li>Balanced partitioning (Potts-style) for multi-chip mapping</li>
      <li>Delay-tolerant links verified via energy/free-energy metrics</li>
      <li>Graph-colored (chromatic) Gibbs at scale</li>
    </ul>
  </div>
  <div class="card">
    <h4>Probabilistic AI & energy-based models</h4>
    <ul>
      <li>Deep Boltzmann networks on hardware with compact topology</li>
      <li>Contrastive Divergence with up to <strong>10M sweeps/update</strong></li>
      <li>Generative capability beyond software baselines</li>
    </ul>
  </div>
  <div class="card">
    <h4>Quantum-inspired optimization</h4>
    <ul>
      <li>All-to-all behavior on sparse fabrics (multiplexed)</li>
      <li>Higher-order couplings (e.g., XORSAT)</li>
      <li>Parallel Tempering / Adaptive PT; non-equilibrium MC</li>
    </ul>
  </div>
</div>

### Impact snapshots
<div class="stat-row">
  <span class="stat-badge">Linear flips/s scaling with # of p-bits</span>
  <span class="stat-badge">50–64B flips/s (measured)</span>
  <span class="stat-badge">6 orders faster vs CPU Gibbs</span>
  <span class="stat-badge">5–18× vs TPU/GPU samplers</span>
  <span class="stat-badge">4,264 p-bits (DBMs)</span>
  <span class="stat-badge">All-to-all + higher-order on sparse IMs</span>
  <span class="stat-badge">Multi-FPGA path to 1M+ nodes</span>
</div>

### Flagship results (concise)
<div class="card-grid">
  <div class="card">
    <h4>Massively parallel sparse Ising machines</h4>
    <div>Linear flips/s with system size; large wins vs CPU/TPU/GPU; correct ground states persist even with faster inexact clocks. <em>Nature Electronics (2022)</em></div>
  </div>
  <div class="card">
    <h4>Deep Boltzmann networks on hardware</h4>
    <div>Hardware-aware DBMs reach software-level accuracy with far fewer parameters; sustained 50–64B flips/s; CD-<em>n</em> up to 10M. <em>Nature Electronics (2024)</em></div>
  </div>
  <div class="card">
    <h4>All-to-all & higher-order on sparse fabrics</h4>
    <div>Multiplexed all-to-all while keeping parallel Gibbs; higher-order interactions improve prefactors on XORSAT. <em>Nature Communications (2024)</em></div>
  </div>
</div>

### Methods I use
<ul class="pill-list">
  <li>Chromatic Gibbs</li>
  <li>Parallel Tempering / Adaptive PT</li>
  <li>Non-equilibrium Monte Carlo</li>
  <li>Balanced partitioning</li>
  <li>Delay-tolerant communication</li>
  <li>All-to-all emulation</li>
  <li>Higher-order couplings</li>
  <li>Energy / free-energy diagnostics</li>
</ul>

### Current directions
- **Million-node p-computers:** latency-aware partitioning and communication with quality retention at scale.  
- **Probabilistic AI at scale:** compact, hardware-efficient energy-based learning for vision and scientific data.  
- **Heterogeneous p-computers:** CMOS + nanomagnets to push flips/J and density.

> Full list of papers is on the **[Publications](/publications/)** page.
<!-- End -->
