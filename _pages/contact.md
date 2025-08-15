---
permalink: /contact/
layout: single
title: "Contact"
author_profile: true
---

<!-- Page-scoped styles (theme-aware) -->
<style>
.grid-2{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:14px;margin:.6rem 0 1.1rem;}
.card{border:1px solid var(--footer-border,#e5e7eb);background:var(--footer-bg,#f8fafc);border-radius:10px;padding:14px;}
.card h3{margin:.1rem 0 .4rem;font-size:1.06rem}
.kv{margin:.25rem 0;}
.kv dt{font-weight:600}
.kv dd{margin:0 0 .4rem 0}
.btn{display:inline-block;font-weight:600;text-decoration:none;border-radius:8px;padding:10px 14px;border:1px solid transparent;transition:transform .02s ease,background-color .2s ease,border-color .2s ease;}
.btn:active{transform:translateY(1px);}
.btn--soft{background:transparent;color:inherit;border-color:var(--footer-border,#e5e7eb)}
.btn-row{display:flex;flex-wrap:wrap;gap:10px;margin-top:.5rem}
@media (max-width:980px){.grid-2{grid-template-columns:1fr}}
address{font-style:normal;line-height:1.5}
.small{font-size:.92rem;opacity:.9}
</style>

<div class="grid-2">
  <div class="card">
    <h3>Email</h3>
    <div class="kv">
      <dt>Primary</dt>
      <dd><a href="mailto:maadit@ucsb.edu">maadit@ucsb.edu</a></dd>
    </div>
    <div class="btn-row">
      <a class="btn btn--soft" href="mailto:maadit@ucsb.edu">Compose Email</a>
      <a class="btn btn--soft" href="https://scholar.google.com/citations?user=KXA0nl4AAAAJ&hl=en">Google Scholar</a>
      <a class="btn btn--soft" href="https://www.linkedin.com/in/navidanjumaadit/">LinkedIn</a>
      <a class="btn btn--soft" href="https://github.com/navidaadit">GitHub</a>
    </div>
    <p class="small" style="margin-top:.6rem">For collaboration or student inquiries, email is best.</p>
  </div>

  <div class="card">
    <h3>Mailing Address</h3>
    <address>
      Department of Electrical &amp; Computer Engineering<br>
      University of California, Santa Barbara<br>
      Santa Barbara, CA, USA
    </address>
  </div>
</div>
