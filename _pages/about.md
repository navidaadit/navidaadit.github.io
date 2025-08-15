---
permalink: /
layout: single
title: ""
author_profile: true
---

<!-- ---------- Page-scoped styles (no global side effects) ---------- -->
<style>
/* Layout tweaks for this page only */
.about-lead { font-size: 1.06rem; line-height: 1.7; margin: .25rem 0 1rem; }
.about-grid { display: grid; grid-template-columns: minmax(0,1fr) minmax(0,1fr); gap: 16px; margin-top: .6rem; }
.about-card {
  border: 1px solid var(--footer-border, #e5e7eb);
  background: var(--footer-bg, #f8fafc);
  border-radius: 10px;
  padding: 14px;
}
.about-card h3 { margin: .2rem 0 .5rem; font-size: 1.05rem; }
.about-list { margin: 0; padding-left: 18px; }
.about-list li { margin: .28rem 0; }
.hr-soft {
  height: 1px; border: 0; background: var(--footer-border, #e5e7eb);
  margin: .9rem 0 .8rem;
}
/* make the hero a touch smaller on large screens */
.hero-img { width: 78% !important; }
/* stack on mobile */
@media (max-width: 980px) {
  .about-grid { grid-template-columns: 1fr; }
  .hero-img { width: 100% !important; }
}
</style>

<!-- HERO as a normal image (no cropping). Lives entirely in the right column. -->
<img src="/images/hero.jpeg" alt="Navid Aadit giving a talk" class="hero-img" />

<p class="cv-row">
  <a class="btn btn--cv" href="/files/Aadit_CV_Fall2025.pdf">Download CV</a>
</p>

<div class="about-lead">
I am a PhD candidate in <strong>Electrical &amp; Computer Engineering</strong> at the <strong>University of California, Santa Barbara</strong> (expected Dec 2025).
</div>

I work on <strong>probabilistic computing</strong> with p-bits and <strong>extreme-scale distributed architectures</strong>, connecting ideas from <strong>statistical physics</strong>, <strong>machine learning</strong>, and <strong>quantum-inspired optimization</strong>.

My recent work scales p-computers across <strong>multi-FPGA systems</strong> with delay-tolerant communication and balanced partitioning to sustain solution quality at unprecedented sizes.

<ul class="keyword-pills">
  <li>Probabilistic computing</li>
  <li>Quantum computing</li>
  <li>Ising/Boltzmann machines</li>
  <li>Distributed chips</li>
  <li>FPGA accelerators</li>
  <li>Energy-based ML</li>
</ul>

<hr class="hr-soft" />

## Research Highlights
- <strong>Distributed probabilistic computing</strong> — Interconnect multi-FPGA / heterogeneous hardware over ultra-low-latency links; ~<strong>1M p-bits</strong> scaling.
- <strong>Probabilistic AI &amp; ML</strong> — Ising/Boltzmann samplers for generative AI, Bayesian inference, and scalable energy-based ML.
- <strong>Quantum-inspired optimization</strong> — Hardware–software co-design blending probabilistic systems with quantum-classical workflows.

<hr class="hr-soft" />

<div class="about-grid">
  <div class="about-card">
    <h3>Key first-author papers</h3>
    <ul class="about-list">
      <li><em>Nature Electronics</em> (2022): <strong>Massively parallel probabilistic computing with sparse Ising machines</strong>.</li>
      <li><em>Nature Communications</em> (2024): <strong>All-to-all reconfigurability with sparse &amp; higher-order Ising machines</strong>.</li>
      <li><em>VLSI Symposium</em> (2023): <strong>Accelerating Adaptive Parallel Tempering with FPGA-based p-bits</strong>.</li>
      <li><em>IEDM</em> (2022): <strong>Experimental evaluation of simulated quantum annealing with MTJ-augmented p-bits</strong>.</li>
      <li><em>IEDM</em> (2021): <strong>Computing with invertible logic: Combinatorial optimization with probabilistic bits</strong>.</li>
    </ul>
  </div>

  <div class="about-card">
    <h3>Recognition</h3>
    <ul class="about-list">
      <li><i class="fas fa-award"></i> <strong>Misha Mahowald Prize (2025)</strong> — <a href="https://www.mahowaldprize.org/prize-awards/prizes-2025">Official Announcement</a> · <a href="https://www.ece.ucsb.edu/news/all/2025/camsaris-opus-lab-misha-mahowald-prize">UCSB News</a></li>
      <li><i class="fas fa-trophy"></i> <strong>Bell Labs Prize (Bronze, 2023)</strong> — <a href="https://engineering.ucsb.edu/news/ece-professor-and-phd-student-win-bronze-medal-bell-labs-prize-competition">UCSB News</a> · <a href="https://www.bell-labs.com/institute/blog/bell-labs-prize-winners-close-the-thz-gap-with-inexpensive-harmonic-sensors/">Bell Labs Blog</a></li>
      <li><i class="fas fa-graduation-cap"></i> <strong>UCSB Graduate Division — PhD Dissertation Fellowship (2025)</strong></li>
    </ul>
  </div>
</div>
