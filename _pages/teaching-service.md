---
permalink: /teaching-service/
layout: single
title: "Teaching & Service"
author_profile: true
---

<!-- Minimal, clean styling just for this page (light-only, no theme vars) -->
<style>
  .section{
    border:1px solid #e5e7eb;
    background:#f8fafc;
    border-radius:10px;
    padding:14px;
    margin:.6rem 0;
  }
  .section h3{margin:.1rem 0 .25rem;color:#111827}
  .role-line{font-size:.92rem;opacity:.8;margin:.1rem 0 .4rem}
  .list{list-style:none;padding:0;margin:.25rem 0}
  .list li{padding:.18rem 0}

  .columns{
    display:grid;
    grid-template-columns:repeat(2,minmax(0,1fr));
    gap:14px;
  }
  @media (max-width:980px){
    .columns{grid-template-columns:1fr}
  }

  /* inline, middot-separated reviewer list — wrap-safe & NOT justified */
  .inline-list{
    list-style:none;
    padding:0;
    margin:.2rem 0;
    display:flex;
    flex-wrap:wrap;
    gap:6px 12px;
    max-width:100%;
    text-align:left !important;
    text-justify:auto !important;
  }
  .inline-list li{
    position:relative;
    white-space:normal;
    overflow-wrap:anywhere;
    word-break:normal;
    max-width:100%;
    line-height:1.4;
    text-align:left !important;
    text-justify:auto !important;
  }
  .inline-list li:not(:last-child)::after{
    content:"•";
    margin-left:12px;
    opacity:.45;
  }
  @media (max-width:540px){
    .inline-list{gap:6px 8px}
    .inline-list li:not(:last-child)::after{margin-left:8px}
  }

  /* keep normal (non-justified) lists inside these light sections */
  .section .list,
  .section .list li{
    text-align:left !important;
    text-justify:auto !important;
  }
</style>

## Teaching

<div class="columns">
  <div class="section">
    <h3>University of California, Santa Barbara (UCSB)</h3>
    <div class="role-line">Role: Teaching Assistant</div>
    <ul class="list">
      <li><strong>ECE 153A / ECE 253</strong> — Hardware/Software Interfaces; Embedded System Design</li>
      <li><strong>ECE 15A</strong> — Fundamentals of Logic Design</li>
    </ul>
  </div>

  <div class="section">
    <h3>University of California, Irvine (UCI)</h3>
    <div class="role-line">Role: Teaching Assistant</div>
    <ul class="list">
      <li><strong>ICS 6B</strong> — Boolean Algebra</li>
      <li><strong>ICS 32</strong> — Python Programming</li>
      <li><strong>ICS 60</strong> — Computer Games &amp; Society</li>
    </ul>
  </div>
</div>

<div class="section">
  <h3>Notre Dame University Bangladesh (NDUB)</h3>
  <ul class="list">
    <li>Lecturer, Department of Computer Science &amp; Engineering (CSE)</li>
    <li>Founder &amp; moderator, NDUB Computer Club</li>
  </ul>
</div>

## Professional Service (Reviewer)

<div class="section">
  <ul class="inline-list">
    <li>IEEE Transactions on Affective Computing</li>
    <li>IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems</li>
    <li>IEEE Transactions on Nanotechnology</li>
    <li>Nature Scientific Reports</li>
    <li>Communications Physics</li>
    <li>IEEE Access</li>
    <li>PLOS ONE</li>
    <li>Digital Discovery</li>
  </ul>
</div>
