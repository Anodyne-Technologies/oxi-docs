---
layout: home
title: OXI Documentation
permalink: /
---

<section class="hero" aria-labelledby="hero-title">
  <h1 id="hero-title">OXI Documentation</h1>
  <p>Build XR with a clean, strongly-typed, path-based API. Unity-first integration, engine-agnostic core.</p>
  <div class="cta-row">
    <a class="btn" href="/manual/">Manual</a>
    <a class="btn" href="/api/">Scripting API</a>
    <a class="btn" href="/devlogs/">Dev Logs</a>
  </div>
</section>

<section class="search" aria-labelledby="search-title">
  <h2 id="search-title">Search</h2>
  <input id="site-search" type="search" placeholder="Search docs…" aria-label="Search docs (press / to focus)" />
  <p class="hint">Tip: press “/” to focus the search box.</p>
</section>

<section class="getting-started" aria-labelledby="gs-title">
  <h2 id="gs-title">Getting Started</h2>
  <ol>
    <li><a href="/manual/overview/">What is OXI?</a></li>
    <li><a href="/manual/installation/">Install &amp; Setup</a></li>
    <li><a href="/manual/quickstart/">Quickstart</a></li>
    <li><a href="/manual/unity/">Unity Integration</a></li>
  </ol>
</section>

<script>
window.addEventListener('keydown', function(event) {
  if (event.key === '/' && document.activeElement !== document.getElementById('site-search')) {
    event.preventDefault();
    var search = document.getElementById('site-search');
    if (search) { search.focus(); }
  }
});
</script>

