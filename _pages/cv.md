---
permalink: /cv/
layout: single
title: "Curriculum Vitae"
author_profile: true
---

<!-- Page-scoped styles (light-only, no theme dependency) -->
<style>
  .cv-intro{
    margin:.25rem 0 1rem;
    font-size:1.02rem;
    line-height:1.6;
    color:#111827;
  }
  .cv-actions{
    display:flex;
    gap:12px;
    flex-wrap:wrap;
    align-items:center;
    margin:.6rem 0 1.2rem;
  }
  .cv-actions a{
    display:inline-block;
    text-decoration:none;
    font-weight:600;
    padding:10px 16px;
    border-radius:8px;
    border:1px solid #3f5fc0;
    transition:background-color .2s ease,border-color .2s ease,transform .02s ease;
    line-height:1.2;
  }
  .cv-actions .btn-view{
    background:#ffffff;
    color:#1f2937;
    border-color:#d1d5db;
  }
  .cv-actions .btn-view:hover{
    background:#f3f4f6;
    border-color:#cbd5e1;
  }
  .cv-actions .btn-download{
    background:#4a6fdd;
    color:#ffffff;
    border-color:#3f5fc0;
  }
  .cv-actions .btn-download:hover{
    background:#3f5fc0;
    border-color:#3552a6;
  }
  .cv-actions a:active{ transform:translateY(1px); }

  .small-note{ font-size:.92rem; opacity:.9; margin-top:.2rem; color:#111827; }

  /* Print-friendly: show links and ensure good contrast */
  @media print{
    .cv-actions a{ color:#000 !important; border-color:#000; background:#fff; }
  }
</style>

<div class="cv-intro">
  View or download the most recent version of my CV:
</div>

<div class="cv-actions">
  <a class="btn-view" href="https://drive.google.com/file/d/12ZX9rrb-iJNACLPJip0xjfp9GKYYN6ZB/view?usp=sharing"
     target="_blank" rel="noopener noreferrer" aria-label="View CV on Google Drive">
     View online (Google Drive)
  </a>
  <a class="btn-download" href="https://drive.google.com/uc?export=download&id=12ZX9rrb-iJNACLPJip0xjfp9GKYYN6ZB"
     rel="noopener" aria-label="Download CV as PDF">
     Download PDF
  </a>
</div>

<p class="small-note">If the preview doesn’t load, use the Download link.</p>
