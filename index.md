---
title: Open Source is Tech Transfer
description: Resources for understanding open source software as technology transfer — for researchers, institutions, and policymakers.
---

<style>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;1,400&family=Source+Serif+4:wght@300;400;600&display=swap');

  body {
    font-family: 'Source Serif 4', Georgia, serif;
    color: #1a1a2e;
    background: #fafaf7;
  }

  .site-hero {
    background: linear-gradient(135deg, #0d2137 0%, #1a4a6b 60%, #0d6e6e 100%);
    color: white;
    padding: 80px 40px 60px;
    margin: -20px -40px 60px;
    position: relative;
    overflow: hidden;
  }

  .site-hero::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -10%;
    width: 600px;
    height: 600px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(255,255,255,0.04) 0%, transparent 70%);
    pointer-events: none;
  }

  .site-hero::after {
    content: '';
    position: absolute;
    bottom: -30px;
    left: 5%;
    width: 300px;
    height: 300px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(13,110,110,0.3) 0%, transparent 70%);
    pointer-events: none;
  }

  .hero-eyebrow {
    font-family: 'Source Serif 4', serif;
    font-weight: 300;
    font-size: 0.85rem;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    opacity: 0.7;
    margin-bottom: 20px;
  }

  .hero-headline {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: clamp(2.2rem, 5vw, 3.8rem);
    font-weight: 700;
    line-height: 1.15;
    margin-bottom: 24px;
    max-width: 700px;
  }

  .hero-headline em {
    font-style: italic;
    color: #7dd4c0;
  }

  .hero-subhead {
    font-size: 1.1rem;
    font-weight: 300;
    line-height: 1.7;
    max-width: 600px;
    opacity: 0.88;
    margin-bottom: 40px;
  }

  .hero-nav {
    display: flex;
    gap: 12px;
    flex-wrap: wrap;
  }

  .btn-primary {
    background: #7dd4c0;
    color: #0d2137;
    padding: 12px 28px;
    border-radius: 2px;
    font-family: 'Source Serif 4', serif;
    font-weight: 600;
    font-size: 0.9rem;
    letter-spacing: 0.05em;
    text-decoration: none;
    display: inline-block;
    transition: background 0.2s;
  }

  .btn-primary:hover { background: #9ee4d4; text-decoration: none; }

  .btn-outline {
    background: transparent;
    color: white;
    padding: 12px 28px;
    border-radius: 2px;
    border: 1px solid rgba(255,255,255,0.4);
    font-family: 'Source Serif 4', serif;
    font-weight: 300;
    font-size: 0.9rem;
    letter-spacing: 0.05em;
    text-decoration: none;
    display: inline-block;
    transition: border-color 0.2s;
  }

  .btn-outline:hover { border-color: white; text-decoration: none; color: white; }

  .stat-strip {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
    gap: 0;
    background: #0d2137;
    color: white;
    margin: 0 -40px 60px;
    padding: 0 40px;
  }

  .stat-item {
    padding: 28px 24px;
    border-right: 1px solid rgba(255,255,255,0.1);
    text-align: center;
  }

  .stat-item:last-child { border-right: none; }

  .stat-number {
    font-family: 'Playfair Display', serif;
    font-size: 2.2rem;
    font-weight: 700;
    color: #7dd4c0;
    display: block;
    line-height: 1;
    margin-bottom: 6px;
  }

  .stat-label {
    font-size: 0.75rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    opacity: 0.65;
    font-weight: 300;
  }

  .section-label {
    font-family: 'Source Serif 4', serif;
    font-weight: 300;
    font-size: 0.75rem;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    color: #0d6e6e;
    margin-bottom: 12px;
    display: block;
  }

  .section-title {
    font-family: 'Playfair Display', serif;
    font-size: clamp(1.6rem, 3vw, 2.4rem);
    font-weight: 700;
    color: #0d2137;
    line-height: 1.2;
    margin-bottom: 20px;
  }

  .section-body {
    font-size: 1.05rem;
    line-height: 1.8;
    color: #3a3a4a;
    font-weight: 300;
    max-width: 680px;
  }

  .thesis-block {
    border-left: 3px solid #0d6e6e;
    padding: 28px 32px;
    background: white;
    box-shadow: 0 2px 24px rgba(13,33,55,0.07);
    margin: 40px 0;
  }

  .thesis-block blockquote {
    font-family: 'Playfair Display', serif;
    font-size: 1.25rem;
    font-style: italic;
    line-height: 1.65;
    color: #0d2137;
    margin: 0;
    border: none;
    padding: 0;
  }

  .thesis-block cite {
    display: block;
    margin-top: 16px;
    font-family: 'Source Serif 4', serif;
    font-size: 0.8rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: #888;
    font-style: normal;
  }

  .two-col {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 40px;
    margin: 40px 0;
  }

  @media (max-width: 700px) { .two-col { grid-template-columns: 1fr; } }

  .card {
    background: white;
    padding: 32px;
    box-shadow: 0 2px 16px rgba(13,33,55,0.06);
    border-top: 3px solid #0d6e6e;
  }

  .card h3 {
    font-family: 'Playfair Display', serif;
    font-size: 1.2rem;
    font-weight: 700;
    color: #0d2137;
    margin-bottom: 12px;
  }

  .card p {
    font-size: 0.95rem;
    line-height: 1.75;
    color: #4a4a5a;
    font-weight: 300;
    margin: 0;
  }

  .presentations-section {
    background: #f0f4f0;
    margin: 60px -40px;
    padding: 60px 40px;
  }

  .presentation-item {
    margin-bottom: 60px;
  }

  .presentation-item:last-child { margin-bottom: 0; }

  .presentation-label {
    font-family: 'Source Serif 4', serif;
    font-weight: 600;
    font-size: 0.8rem;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: #0d6e6e;
    margin-bottom: 8px;
  }

  .presentation-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.5rem;
    font-weight: 700;
    color: #0d2137;
    margin-bottom: 20px;
  }

  .slides-wrapper {
    position: relative;
    width: 100%;
    padding-top: 59.27%;
    overflow: hidden;
    box-shadow: 0 8px 40px rgba(13,33,55,0.15);
  }

  .slides-wrapper iframe {
    position: absolute;
    top: 0; left: 0;
    width: 100%; height: 100%;
    border: none;
  }

  .about-strip {
    background: #0d2137;
    color: white;
    margin: 60px -40px 0;
    padding: 60px 40px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 60px;
    align-items: center;
  }

  @media (max-width: 700px) { .about-strip { grid-template-columns: 1fr; } }

  .about-strip h2 {
    font-family: 'Playfair Display', serif;
    font-size: 2rem;
    color: white;
    margin-bottom: 20px;
  }

  .about-strip p {
    font-size: 0.95rem;
    line-height: 1.8;
    opacity: 0.8;
    font-weight: 300;
    margin-bottom: 24px;
  }

  .about-strip a.btn-primary { display: inline-block; }

  .ositt-info h3 {
    font-family: 'Playfair Display', serif;
    font-size: 1.2rem;
    color: #7dd4c0;
    margin-bottom: 12px;
  }

  .ositt-info p {
    font-size: 0.9rem;
    opacity: 0.7;
    margin-bottom: 0;
  }

  hr { border: none; border-top: 1px solid #e0e0d8; margin: 48px 0; }
</style>

<div class="site-hero">
  <div class="hero-eyebrow">A Framework for Academic Technology Transfer</div>
  <h1 class="hero-headline">Open Source <em>is</em><br>Tech Transfer</h1>
  <p class="hero-subhead">University technology transfer offices are uniquely positioned to support open source software — and open source practices are an efficient, often optimal mechanism for translating computational research to the world.</p>
  <div class="hero-nav">
    <a href="about" class="btn-primary">About This Project</a>
    <a href="#presentations" class="btn-outline">View Presentations</a>
  </div>
</div>

<div class="stat-strip">
  <div class="stat-item">
    <span class="stat-number">32</span>
    <span class="stat-label">TTOs & OSPOs in Working Group</span>
  </div>
  <div class="stat-item">
    <span class="stat-number">$12.2T</span>
    <span class="stat-label">Estimated Value of Open Source</span>
  </div>
  <div class="stat-item">
    <span class="stat-number">1980</span>
    <span class="stat-label">Bayh-Dole Act Origin</span>
  </div>
  <div class="stat-item">
    <span class="stat-number">CC0</span>
    <span class="stat-label">Freely Licensed Content</span>
  </div>
</div>

<span class="section-label">The Core Argument</span>
<h2 class="section-title">Why Open Source Belongs<br>in the TTO Mission</h2>

<p class="section-body">University technology transfer offices were founded to translate research into public benefit. For decades, that has meant patents and proprietary licensing. But as software has extended a computational layer across nearly all of basic scientific research, a gap has opened: open source — the dominant mode of software-driven discovery — has been largely left out of the TTO mission.</p>

<div class="thesis-block">
  <blockquote>"Open source technology transfer drives impact by accelerating scientific discovery, enabling industry collaboration, promoting broad public awareness and adoption, facilitating commercialization and sustainability of open source projects, fostering startup creation, attracting external funding opportunities, advancing workforce development, catalyzing regional economic growth, and enhancing the reputation of academic researchers and their institutions."</blockquote>
  <cite>— OSiTT Working Group Definition of Impact</cite>
</div>

<p class="section-body">The policy rationale for statutes like the Bayh-Dole Act — promoting utilization of federally funded inventions, ensuring public availability, protecting against nonuse — is met by open source practices at least as well as by patent licensing for computational technologies. TTOs are the organizations best positioned to facilitate this work.</p>

<hr>

<span class="section-label">The Framework</span>
<h2 class="section-title">Five Areas Where TTOs<br>Can Support Open Source</h2>

<div class="two-col">
  <div class="card">
    <h3>Open Source Reporting</h3>
    <p>TTOs can apply the same relationship-building resources used to capture invention disclosures to tracking open source projects. Quantifying open source software at a university is a prerequisite to measuring its technology transfer impact.</p>
  </div>
  <div class="card">
    <h3>Open Source Licensing</h3>
    <p>TTOs are in a strong position to assist researchers with license compliance, choice of license based on project objectives, and establishing governance structures like contributor license agreements and contribution guidelines.</p>
  </div>
  <div class="card">
    <h3>Promotion</h3>
    <p>TTO websites can feature open source projects alongside traditional technologies, with links to public repositories, publications, and datasets — lowering the barrier for potential partners to evaluate university computational research.</p>
  </div>
  <div class="card">
    <h3>Community Building</h3>
    <p>Just as TTOs support startups with market research and customer discovery, they can help open source projects develop strategies for adoption, manage feature requests, and build contributor communities.</p>
  </div>
</div>

<div class="card" style="border-top-color: #1a4a6b; margin-bottom: 40px;">
  <h3>Sustainability</h3>
  <p>TTOs support business model ideation for traditional startups. The same expertise applies to open source: advising on commercial open source (COSS) startup models, sponsor-funded models, and open core licensing as viable research endpoints.</p>
</div>

<div class="presentations-section" id="presentations">
  <span class="section-label">Presentations</span>
  <h2 class="section-title" style="margin-bottom: 48px;">OSiTT Working Group Slides</h2>

  <div class="presentation-item">
    <div class="presentation-label">Presentation 01</div>
    <div class="presentation-title">The Role of TTOs in Supporting Open Source Translation</div>
    <div class="slides-wrapper">
      <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vT1OYa7mMOvr3lteEj1wRUw72s6OOSHbMsOLlALq7l1BIE6l-q8rsQoUY-MDe-m9Q/pubembed?start=false&loop=true&delayms=3000" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
    </div>
  </div>

  <div class="presentation-item">
    <div class="presentation-label">Presentation 02</div>
    <div class="presentation-title">The Impact of Open Source on Software Licensing</div>
    <div class="slides-wrapper">
      <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vQSTPN6iwiuLT4X6AVmK8ylSRhBlWMcWs7u9VlBvIMxp9Ye4uxGm8X0f-DaJWy3GQ/pubembed?start=false&loop=true&delayms=3000" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
    </div>
  </div>

  <div class="presentation-item">
    <div class="presentation-label">Presentation 03</div>
    <div class="presentation-title">Solving for Open Source in Technology Transactions</div>
    <div class="slides-wrapper">
      <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vR_ouGcTSvYQB8anVnSW4De7RpIInn68qHWejnpRW98CizOLnfar9kJV-uh_inqnQ/pubembed?start=false&loop=true&delayms=3000" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
    </div>
  </div>
</div>

<div class="about-strip">
  <div>
    <h2>About This Project</h2>
    <p>This site is a resource developed through the Open Source is Tech Transfer (OSiTT) working group — a community of 32 TTOs, open source programs offices, and related organizations across the United States and abroad who work with open source software.</p>
    <p>The project is led by Andrew Wichmann at Johns Hopkins University, with co-authors Megan Forbes and Ashwathi Iyer (University of Michigan).</p>
    <a href="about" class="btn-primary">Learn More</a>
  </div>
  <div class="ositt-info">
    <h3>The OSiTT Working Group</h3>
    <p>Monthly discussions throughout 2025 brought together practitioners from Arizona, Chicago, CMU, GW, Illinois, JHU, LSU, MIT, Michigan, NYU, Oregon State, RIT, Stanford, Yale, and institutions in Ireland, Belgium, and beyond.</p>
  </div>
</div>
