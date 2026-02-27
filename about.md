---
title: About — Open Source is Tech Transfer
description: About the OSiTT working group and the people behind this project.
---

<style>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;1,400&family=Source+Serif+4:wght@300;400;600&display=swap');

  body {
    font-family: 'Source Serif 4', Georgia, serif;
    color: #1a1a2e;
    background: #fafaf7;
  }

  .page-hero {
    background: linear-gradient(135deg, #0d2137 0%, #1a4a6b 60%, #0d6e6e 100%);
    color: white;
    padding: 80px 40px 60px;
    margin: -20px -40px 60px;
    position: relative;
    overflow: hidden;
  }

  .page-hero::before {
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
    font-size: clamp(2rem, 4vw, 3.2rem);
    font-weight: 700;
    line-height: 1.15;
    margin-bottom: 20px;
  }

  .hero-subhead {
    font-size: 1.05rem;
    font-weight: 300;
    line-height: 1.7;
    max-width: 600px;
    opacity: 0.88;
    margin-bottom: 32px;
  }

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
  }

  .btn-outline:hover { border-color: white; text-decoration: none; color: white; }

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
    font-size: clamp(1.6rem, 3vw, 2.2rem);
    font-weight: 700;
    color: #0d2137;
    line-height: 1.2;
    margin-bottom: 20px;
  }

  .prose {
    font-size: 1.05rem;
    line-height: 1.85;
    color: #3a3a4a;
    font-weight: 300;
    max-width: 700px;
    margin-bottom: 20px;
  }

  hr { border: none; border-top: 1px solid #e0e0d8; margin: 52px 0; }

  .author-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 28px;
    margin: 36px 0;
  }

  .author-card {
    background: white;
    padding: 32px;
    box-shadow: 0 2px 16px rgba(13,33,55,0.06);
    border-top: 3px solid #0d6e6e;
  }

  .author-name {
    font-family: 'Playfair Display', serif;
    font-size: 1.2rem;
    font-weight: 700;
    color: #0d2137;
    margin-bottom: 4px;
  }

  .author-affiliation {
    font-size: 0.8rem;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: #0d6e6e;
    margin-bottom: 16px;
    font-weight: 300;
  }

  .author-bio {
    font-size: 0.92rem;
    line-height: 1.75;
    color: #4a4a5a;
    font-weight: 300;
    margin: 0;
  }

  .highlight-box {
    border-left: 3px solid #0d6e6e;
    padding: 28px 32px;
    background: white;
    box-shadow: 0 2px 24px rgba(13,33,55,0.07);
    margin: 36px 0;
  }

  .highlight-box p {
    font-family: 'Playfair Display', serif;
    font-size: 1.15rem;
    font-style: italic;
    line-height: 1.65;
    color: #0d2137;
    margin: 0;
  }

  .wg-section {
    background: #f0f4f0;
    margin: 60px -40px;
    padding: 60px 40px;
  }

  .wg-institutions {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 28px;
  }

  .wg-tag {
    background: white;
    border: 1px solid #d0d8d0;
    color: #0d2137;
    padding: 6px 14px;
    font-size: 0.82rem;
    font-weight: 300;
    letter-spacing: 0.05em;
    border-radius: 2px;
  }

  .paper-strip {
    background: #0d2137;
    color: white;
    margin: 60px -40px 0;
    padding: 52px 40px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 40px;
    flex-wrap: wrap;
  }

  .paper-strip h2 {
    font-family: 'Playfair Display', serif;
    font-size: 1.6rem;
    color: white;
    margin-bottom: 10px;
  }

  .paper-strip p {
    font-size: 0.9rem;
    opacity: 0.7;
    font-weight: 300;
    max-width: 500px;
    margin: 0;
  }

  .btn-primary {
    background: #7dd4c0;
    color: #0d2137;
    padding: 14px 32px;
    border-radius: 2px;
    font-family: 'Source Serif 4', serif;
    font-weight: 600;
    font-size: 0.9rem;
    letter-spacing: 0.05em;
    text-decoration: none;
    display: inline-block;
    white-space: nowrap;
  }

  .btn-primary:hover { background: #9ee4d4; text-decoration: none; }
</style>

<div class="page-hero">
  <div class="hero-eyebrow">About This Project</div>
  <h1 class="hero-headline">Open Source is Tech Transfer</h1>
  <p class="hero-subhead">A working group of technology transfer offices and open source programs offices making the case that open source software is a legitimate — and often optimal — mechanism for translating university research.</p>
  <a href="/" class="btn-outline">← Back to Home</a>
</div>

<span class="section-label">The Project</span>
<h2 class="section-title">Why This Work Matters</h2>

<p class="prose">University technology transfer offices (TTOs) were created to translate research into public benefit. For decades, that has meant patents and proprietary licensing — an approach formalized by the Bayh-Dole Act of 1980. But as software has become the infrastructure of modern scientific research, a gap has grown: open source software, the dominant mode of computational discovery, has largely been left outside the TTO mission.</p>

<p class="prose">Open source is not the absence of technology transfer — it is technology transfer by another means. When a university releases software under an open source license, it is granting a license to copyrights and often patent rights to the public. TTOs are the organizations designated to license IP at universities. They should also be responsible for open source licenses.</p>

<div class="highlight-box">
  <p>"One would be hard-pressed to find any piece of scientific literature published today that has not been supported in some way by at least a dozen if not more open source software projects."</p>
</div>

<p class="prose">This site is a resource for the technology transfer community — practitioners, researchers, administrators, and policymakers — who want to understand how open source fits within the TTO mission and how to build organizational capacity to support it.</p>

<hr>

<span class="section-label">The Authors</span>
<h2 class="section-title">Who We Are</h2>

<div class="author-grid">
  <div class="author-card">
    <div class="author-name">Andrew Wichmann</div>
    <div class="author-affiliation">Johns Hopkins University</div>
    <p class="author-bio">Andrew Wichmann works at Johns Hopkins Technology Ventures and has been a convener of the OSiTT working group since its founding. His work focuses on the intersection of open source software, intellectual property, and technology transfer policy.</p>
  </div>
  <div class="author-card">
    <div class="author-name">Megan Forbes</div>
    <div class="author-affiliation">Johns Hopkins University</div>
    <p class="author-bio">Megan Forbes is a co-author of the OSiTT framework and brings expertise in open source community strategy and sustainability, including co-authorship of <em>It Takes a Village: Open Source Software Sustainability</em>.</p>
  </div>
  <div class="author-card">
    <div class="author-name">Ashwathi Iyer</div>
    <div class="author-affiliation">University of Michigan</div>
    <p class="author-bio">Ashwathi Iyer is a co-author based at the University of Michigan's Innovation Partnerships office, which operates the Michigan Open Source Software (MOSS) program — one of the leading university open source programs in the United States.</p>
  </div>
</div>

<div class="wg-section">
  <span class="section-label">The Community</span>
  <h2 class="section-title">The OSiTT Working Group</h2>

  <p class="prose" style="max-width: 680px;">This work was developed through monthly discussions throughout 2025 with a working group of 32 TTOs, open source programs offices, and related organizations across the United States and abroad. The group's goal is to build shared vocabulary, metrics, and frameworks for open source technology transfer — and to advocate for its formal inclusion in the TTO mission.</p>

  <div class="wg-institutions">
    <span class="wg-tag">Arizona</span>
    <span class="wg-tag">University of Chicago</span>
    <span class="wg-tag">Carnegie Mellon</span>
    <span class="wg-tag">CURIOSS</span>
    <span class="wg-tag">George Washington University</span>
    <span class="wg-tag">University of Illinois</span>
    <span class="wg-tag">Johns Hopkins University</span>
    <span class="wg-tag">JHU Applied Physics Lab</span>
    <span class="wg-tag">LSU</span>
    <span class="wg-tag">Mass General Brigham</span>
    <span class="wg-tag">University of Michigan</span>
    <span class="wg-tag">MIT</span>
    <span class="wg-tag">NYU Langone</span>
    <span class="wg-tag">Oregon State</span>
    <span class="wg-tag">RIT</span>
    <span class="wg-tag">Stanford</span>
    <span class="wg-tag">Trinity College Dublin</span>
    <span class="wg-tag">UAB</span>
    <span class="wg-tag">UC Davis</span>
    <span class="wg-tag">UC Santa Cruz</span>
    <span class="wg-tag">UC San Diego</span>
    <span class="wg-tag">University of Minnesota</span>
    <span class="wg-tag">UNC</span>
    <span class="wg-tag">UT Austin</span>
    <span class="wg-tag">UT Southwestern</span>
    <span class="wg-tag">UTEP</span>
    <span class="wg-tag">University of Vermont</span>
    <span class="wg-tag">University of Washington</span>
    <span class="wg-tag">Vrije Universiteit Brussel</span>
    <span class="wg-tag">Yale</span>
  </div>
</div>

<div class="paper-strip">
  <div>
    <h2>Read the Position Paper</h2>
    <p>"Standardizing Open Source Impact Metrics: A Framework for Academic Technology Transfer Offices" — Forbes, Iyer, and Wichmann, 2026.</p>
  </div>
  <a href="paper" class="btn-primary">Read the Paper →</a>
</div>
