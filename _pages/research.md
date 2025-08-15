---
permalink: /research/
layout: single
title: "Research"
author_profile: true
---

<style>
/* --- lightweight page-scoped styles (safe with your theme) --- */
.research-lead { font-size:1.05rem; line-height:1.6; margin: .25rem 0 1.25rem 0; }
.card-grid { display:grid; grid-template-columns: repeat(3, minmax(0,1fr)); gap:14px; margin:.75rem 0 1.25rem 0; }
.card { border:1px solid var(--footer-border, #e5e7eb); border-radius:10px; padding:14px 14px 12px; background: var(--footer-bg, #f8fafc); }
.card h4 { margin:.1rem 0 .35rem 0; font-size:1.02rem; }
.stat-row { display:flex; flex-wrap:wrap; gap:8px; margin:.35rem 0 1.1rem; }
.stat-badge { font-size:.9rem; padding:6px 10px; border-radius:999px; border:1px solid var(--tag-border, #e5e7eb); background:var(--tag-bg, #f3f4f6); color:var(--tag-fg, #111827); white-space:nowrap; }
.pill-list { list-style:none; padding:0; margin:.1rem 0 .9rem 0; display:flex; flex-wrap:wrap; gap:6px 8px; }
.pill-list li { font-size:.9rem; padding:6px 10px; border-radius:999px; border:1px solid var(--tag-border, #e5e7eb); background:var(--tag-bg, #f3f4f6); color:var(--tag-fg, #111827); white-space:nowrap; }
.section-h { margin-top:.6rem; }
@media (max-width: 980px){ .card-grid{grid-template-columns:1fr;} }
</style>

<div class="research-lead">
I build <strong>probabilistic computers (p-computers)</strong> and <strong>distributed architectures</strong> for fast sampling, inference, and hard optimization — from single FPGAs to <strong>multi-FPGA</strong> fabrics and toward <strong>million-node</strong> scale.
</div>

### Focus areas
<div class="card-grid">
  <div class="card">
    <h4>Distributed p-computers</h4>
    <ul>
      <li>Balanced partitioning & delay-tolerant links</li>
      <li>Graph-colored (chromatic) Gibbs at scale</li>
      <li>Roadmap to <strong>1M+ p-bits</strong></li>
    </ul>
  </div>
  <div class="card">
    <h4>Probabilistic AI & EBMs</h4>
    <ul>
      <li>Hardware-aware DBMs / EBMs</li>
      <li>CD-<em>n</em> with <strong>10M sweeps/update</strong></li>
      <li>Generative sampling beyond software baselines</li>
    </ul>
  </div>
  <div class="card">
    <h4>Quantum-inspired optimization</h4>
    <ul>
      <li>All-to-all on sparse fabrics</li>
      <li>Higher-order couplings (XORSAT)</li>
      <li>PT/APT & non-equilibrium acceleration</li>
    </ul>
  </div>
</div>

### Impact snapshots
<div class="stat-row">
  <span class="stat-badge">50–64B flips/s</span>
  <span class="stat-badge">6 orders faster vs CPU Gibbs</span>
  <span class="stat-badge">5–18× vs TPU/GPU samplers</span>
  <span class="stat-badge">4,264 p-bits (DBMs)</span>
  <span class="stat-badge">All-to-all + higher-order on sparse IMs</span>
  <span class="stat-badge">Multi-FPGA path to 1M+</span>
</div>

### Selected results (one-liners)
<div class="card-grid">
  <div class="card">
    <h4>Massively parallel sparse Ising machines</h4>
    <div>Linear flips/s scaling with p-bits; strong wins vs CPU/TPU/GPU; correct ground states even with faster (inexact) clocks. <em>Nature Electronics (2022)</em></div>
  </div>
  <div class="card">
    <h4>Training deep Boltzmann networks on hardware</h4>
    <div>DBMs on FPGA achieve software-level accuracy with <em>far</em> fewer params; sustained 50–64B flips/s; CD-<em>n</em> up to 10M. <em>Nature Electronics (2024)</em></div>
  </div>
  <div class="card">
    <h4>All-to-all & higher-order on sparse fabrics</h4>
    <div>Multiplexed all-to-all while keeping parallel Gibbs; higher-order improves prefactors on XORSAT. <em>Nature Communications (2024)</em></div>
  </div>
</div>

### How I approach new problems
<ul class="pill-list">
  <li>Chromatic Gibbs</li><li>Adaptive Parallel Tempering</li><li>Non-equilibrium MC</li>
  <li>Balanced partitioning</li><li>Delay-tolerant links</li><li>All-to-all emulation</li>
  <li>Higher-order couplings</li><li>Energy / free-energy diagnostics</li>
</ul>

### Current directions
- **Million-node p-computers:** latency-aware partitioning with quality retention.  
- **Probabilistic AI at scale:** compact EBMs/DBMs for vision & scientific data.  
- **Heterogeneous p-computers:** CMOS + nanomagnets for flips/J gains.

> Full papers and PDFs are on the **[Publications](/publications/)** page.
