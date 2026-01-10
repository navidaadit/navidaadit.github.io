---
permalink: /research/
layout: single
title: "Research"
author_profile: true
---

<!-- Page-scoped styles (light-only; no theme variables) -->
<style>
  .research-lead{font-size:1.06rem;line-height:1.65;margin:.25rem 0 1.15rem;color:#111827;}

  .grid-3{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:14px;margin:.75rem 0 1.2rem;}

  .card{border:1px solid #e5e7eb;border-radius:10px;padding:14px;background:#f7fafc;}
  .card h4{margin:.1rem 0 .35rem;font-size:1.02rem;color:#111827;}

  .stat-row{display:flex;flex-wrap:wrap;gap:8px;margin:.35rem 0 1.1rem;}
  .stat-badge{
    font-size:.9rem;padding:6px 10px;border-radius:999px;
    border:1px solid #e5e7eb;background:#f3f4f6;color:#111827;white-space:nowrap;
  }

  .pill-list{list-style:none;padding:0;margin:.1rem 0 .9rem 0;display:flex;flex-wrap:wrap;gap:6px 8px;}
  .pill-list li{
    font-size:.9rem;padding:6px 10px;border-radius:999px;
    border:1px solid #e5e7eb;background:#f3f4f6;color:#111827;white-space:nowrap;
  }

  .small-note{font-size:.92rem;opacity:.9;color:#111827}
  abbr[title]{text-decoration:none;border:0;cursor:help}

  /* Spotlight grid (2×2). Card/image rules live in global CSS. */
  .gallery-2x2{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:12px;margin:.6rem 0 1.2rem;}
  @media (max-width:980px){.grid-3,.gallery-2x2{grid-template-columns:1fr;}}

  /* Centered, equal-height captions */
  .gallery-2x2 .figure-card{display:flex;flex-direction:column;}
  .gallery-2x2 .figure-card img{flex:0 0 auto;}
  .gallery-2x2 .figure-card figcaption,
  .gallery-2x2 .figure-card .figcap{
    text-align:center !important;margin-top:6px;font-size:.9rem;line-height:1.35;color:#475569;
    display:-webkit-box;-webkit-box-orient:vertical;-webkit-line-clamp:2;overflow:hidden;min-height:calc(1.35em * 2);
  }
</style>

<div class="research-lead">
My current work supports the <strong>Scale AI</strong> effort under the <strong>Microelectronics Commons</strong> program, focused on <strong>3D chip design execution</strong> and <strong>system measurement &amp; verification</strong> for large-scale “Illusion” multi-chiplet designs.<br><br>
Previously, I built <strong>CMOS/FPGA systems</strong> for <strong>probabilistic computing</strong> with <abbr title="probabilistic bit (binary stochastic neuron)">p-bits</abbr> (<strong>Ising/Boltzmann machines</strong>) and <strong>distributed architectures</strong> for fast <strong>sampling</strong>, <strong>learning</strong>, and <strong>quantum-inspired optimization</strong>.
</div>

## Research areas

<div class="grid-3">
  <div class="card">
    <h4>3D multi-chip systems & verification</h4>
    <ul>
      <li>3D chip design execution and integration workflows</li>
      <li>System measurement &amp; validation of silicon/prototypes</li>
      <li>Verification strategies for large “Illusion” multi-chiplet systems</li>
    </ul>
  </div>
  <div class="card">
    <h4>Robust system measurement & bring-up</h4>
    <ul>
      <li>End-to-end measurement planning (test hooks → metrics)</li>
      <li>Debug workflows spanning RTL/emulation to lab instruments</li>
      <li>Scaling-aware validation: corner cases, failure modes, and observability</li>
    </ul>
  </div>
  <div class="card">
    <h4>Probabilistic computing (prior work)</h4>
    <ul>
      <li>p-bit based Ising/Boltzmann machines on CMOS/FPGA</li>
      <li>Distributed, latency-tolerant fabrics for extreme-scale sampling</li>
      <li>Applications: optimization, energy-based ML, AI sampling</li>
    </ul>
  </div>
</div>

## Full-stack focus

<div class="grid-3">
  <div class="card">
    <h4>Silicon / system layer</h4>
    <ul>
      <li>3D integration constraints: testability, observability, bring-up</li>
      <li>Measurement-driven iteration loops (hardware ↔ models)</li>
      <li>Robustness: fault isolation and scaling bottlenecks</li>
    </ul>
  </div>
  <div class="card">
    <h4>Architecture</h4>
    <ul>
      <li>Multi-chiplet partitioning and communication-aware design</li>
      <li>Verification-friendly interfaces and debug visibility</li>
      <li>Distributed probabilistic fabrics: async, delay-tolerant links (prior)</li>
    </ul>
  </div>
  <div class="card">
    <h4>Algorithms / workflows</h4>
    <ul>
      <li>Validation workflows across abstraction levels</li>
      <li>Performance/robustness characterization with system-level metrics</li>
      <li>SA/PT/ICM/SQA and hardware-aware learning loops (prior)</li>
    </ul>
  </div>
</div>

## Selected figures of merit (prior p-computer work)

<div class="stat-row">
  <span class="stat-badge">1500B flips/s (measured)</span>
  <span class="stat-badge">Up to 6 orders vs. CPU Gibbs</span>
  <span class="stat-badge">≈100× vs. GPU/TPU (flips/s &amp; energy)</span>
  <span class="stat-badge">6-FPGA UCSB: ~50k p-bits (async links)</span>
  <span class="stat-badge">Synthesized 1M p-bits on 18× VP1902 (Siemens)</span>
  <span class="stat-badge">4,264 p-bits / ≈30k params (DBM)</span>
</div>

## Spotlight (selected prior work)

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
    <figcaption class="figcap">Higher-order IMs &amp; all-to-all approach — <em>Nature Comm.</em> (2024)</figcaption>
  </figure>

  <!-- Rack photo: make it fill the card (no bottom whitespace) -->
  <figure class="figure-card fill">
    <img src="/images/research/5-fpga-setup.jpeg" alt="UCSB multi-FPGA p-computer (rack)">
    <figcaption class="figcap">UCSB multi-FPGA p-computer (~50k p-bits) — lab setup</figcaption>
  </figure>
</div>

## Methods I use

<ul class="pill-list">
  <li>3D chip integration workflows</li>
  <li>System measurement &amp; characterization</li>
  <li>Hardware validation &amp; debug (RTL → system)</li>
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

- <strong>3D chips & multi-chiplet verification</strong>: design execution plus system measurement/verification for large-scale “Illusion” multi-chiplet systems.  
- <strong>Robust, scalable measurement</strong>: validation workflows that remain effective as systems scale in complexity and integration density.  
- <strong>Cross-layer co-design</strong>: interfaces and architectures shaped by what is measurable, verifiable, and debuggable in real hardware.

<div class="small-note">
Full publication list: <a href="/publications/">Publications</a>
</div>
