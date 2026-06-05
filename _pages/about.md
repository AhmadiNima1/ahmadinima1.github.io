---
layout: about
title: Nima Ahmadi, PhD
permalink: /
subtitle: Human Factors Engineer & Researcher

announcements:
  enabled: false
  scrollable: true
  limit: 1

latest_posts:
  enabled: false
  scrollable: true
  limit: 3

selected_papers: false
social: true
---

<style>
  .post-header:has(+ article .home-page) {
    display: none;
  }

  .home-page {
    color: var(--global-text-color);
  }

  .home-page .home-hero {
    margin: 1rem 0 2.75rem;
    padding: 2.25rem 0 1.75rem;
    border-bottom: 1px solid var(--global-divider-color);
  }

  .home-page .home-hero h1 {
    margin-bottom: 0.45rem;
    color: var(--global-text-color);
    font-size: 2.65rem;
    line-height: 1.1;
    font-weight: 700;
  }

  .home-page .home-hero .home-role {
    margin-bottom: 1.2rem;
    color: var(--global-theme-color);
    font-size: 1.15rem;
    font-weight: 600;
  }

  .home-page .home-hero .home-statement {
    max-width: 790px;
    margin-bottom: 0;
    color: var(--global-text-color);
    font-size: 1.08rem;
    line-height: 1.7;
  }

  .home-page .home-section {
    margin-bottom: 2.75rem;
  }

  .home-page .home-section h2 {
    margin-bottom: 1.15rem;
    color: var(--global-text-color);
    font-size: 1.45rem;
    font-weight: 700;
  }

  .home-page .what-i-do-grid {
    display: grid;
    grid-template-columns: repeat(6, minmax(0, 1fr));
    gap: 1rem;
  }

  .home-page .what-i-do-grid .home-card {
    grid-column: span 2;
  }

  .home-page .home-card {
    display: flex;
    flex-direction: column;
    height: 100%;
    padding: 1.35rem;
    background: var(--global-card-bg-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
  }

  .home-page .home-card-number {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 2rem;
    height: 2rem;
    margin-bottom: 0.9rem;
    color: var(--global-theme-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0;
  }

  .home-page .home-card-top {
    display: flex;
    align-items: center;
    gap: 0.55rem;
    margin-bottom: 0.9rem;
  }

  .home-page .home-card-top .home-card-number {
    margin-bottom: 0;
  }

  .home-page .home-card-icon {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 2rem;
    height: 2rem;
    color: var(--global-theme-color);
    background: var(--global-bg-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    font-size: 0.85rem;
  }

  .home-page .home-card h3 {
    margin-bottom: 0.7rem;
    color: var(--global-text-color);
    font-size: 1rem;
    line-height: 1.35;
    font-weight: 700;
  }

  .home-page .home-card p {
    margin-bottom: 1rem;
    color: var(--global-text-color);
    font-size: 0.95rem;
    line-height: 1.65;
  }

  .home-page .method-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-top: 0.85rem;
  }

  .home-page .home-card .method-tags {
    margin-top: auto;
  }

  .home-page .method-tag {
    display: inline-flex;
    align-items: center;
    padding: 0.28rem 0.55rem;
    color: var(--global-text-color);
    background: var(--global-bg-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    font-size: 0.82rem;
    line-height: 1.25;
  }

  html:not([data-theme="dark"]) .home-page,
  html:not([data-theme="dark"]) .home-page p,
  html:not([data-theme="dark"]) .home-page h1,
  html:not([data-theme="dark"]) .home-page h2,
  html:not([data-theme="dark"]) .home-page h3,
  html:not([data-theme="dark"]) .home-page .home-card p,
  html:not([data-theme="dark"]) .home-page .method-tag {
    color: #333333;
  }

  html:not([data-theme="dark"]) .home-page .home-card {
    background: #fafafa;
    border-color: #dedede;
  }

  html:not([data-theme="dark"]) .home-page .home-card-number {
    color: #333333;
    background: #ffffff;
    border-color: #d6d6d6;
  }

  html:not([data-theme="dark"]) .home-page .home-card-icon {
    color: #3f5870;
    background: #ffffff;
    border-color: #d6d6d6;
  }

  html:not([data-theme="dark"]) .home-page .method-tag {
    background: #ffffff;
    border-color: #d8d8d8;
  }

  @media (min-width: 901px) {
    .home-page .what-i-do-grid .home-card:nth-child(4) {
      grid-column: 2 / span 2;
    }

    .home-page .what-i-do-grid .home-card:nth-child(5) {
      grid-column: 4 / span 2;
    }
  }

  @media (max-width: 900px) {
    .home-page .what-i-do-grid {
      grid-template-columns: 1fr;
    }

    .home-page .what-i-do-grid .home-card {
      grid-column: auto;
    }

    .home-page .home-hero h1 {
      font-size: 2.15rem;
    }
  }
</style>

<div class="home-page">
  <section class="home-hero">
    <h1>Nima Ahmadi, PhD</h1>
    <p class="home-role">Human Factors Engineer &amp; Researcher</p>
    <p class="home-statement">
      I study how people interact with complex healthcare, aviation, and safety-critical systems, using human factors methods,
      experimental design, multimodal sensing, statistical analysis, and AI-enabled modeling to support safer and more usable
      technologies.
    </p>
  </section>

  <section class="home-section">
    <h2>What I Do</h2>
    <div class="what-i-do-grid">
      <article class="home-card">
        <div class="home-card-top" aria-hidden="true">
          <span class="home-card-number">01</span>
          <span class="home-card-icon"><i class="fa-solid fa-flask"></i></span>
        </div>
        <h3>Research Design &amp; Study Planning</h3>
        <p>
          Designing human-subject, simulation, naturalistic, and observational studies using quantitative, qualitative, and
          mixed-methods approaches to generate evidence for system improvement.
        </p>
        <div class="method-tags" aria-label="Methods">
          <span class="method-tag">DOE</span>
          <span class="method-tag">A/B testing</span>
          <span class="method-tag">survey design</span>
          <span class="method-tag">simulation studies</span>
          <span class="method-tag">naturalistic studies</span>
          <span class="method-tag">mixed-methods</span>
          <span class="method-tag">mixed-effects modeling</span>
        </div>
      </article>

      <article class="home-card">
        <div class="home-card-top" aria-hidden="true">
          <span class="home-card-number">02</span>
          <span class="home-card-icon"><i class="fa-solid fa-user-check"></i></span>
        </div>
        <h3>Human Factors, UX/UI &amp; Usability Research</h3>
        <p>
          Evaluating user needs, workflows, interfaces, and task performance through usability testing, UX/UI research, task
          analysis, observational studies, and use-related risk assessment.
        </p>
        <div class="method-tags" aria-label="Methods">
          <span class="method-tag">usability testing</span>
          <span class="method-tag">UX/UI research</span>
          <span class="method-tag">task analysis</span>
          <span class="method-tag">workflow analysis</span>
          <span class="method-tag">risk assessment</span>
          <span class="method-tag">formative/summative evaluation</span>
        </div>
      </article>

      <article class="home-card">
        <div class="home-card-top" aria-hidden="true">
          <span class="home-card-number">03</span>
          <span class="home-card-icon"><i class="fa-solid fa-eye"></i></span>
        </div>
        <h3>Human Behavior &amp; Performance Assessment</h3>
        <p>
          Assessing attention, workload, stress, decision-making, and performance using eye tracking, wearable sensors,
          physiological data, behavioral data, and performance measures.
        </p>
        <div class="method-tags" aria-label="Methods">
          <span class="method-tag">eye tracking</span>
          <span class="method-tag">wearable sensing</span>
          <span class="method-tag">workload</span>
          <span class="method-tag">stress</span>
          <span class="method-tag">behavioral data</span>
          <span class="method-tag">performance measures</span>
        </div>
      </article>

      <article class="home-card">
        <div class="home-card-top" aria-hidden="true">
          <span class="home-card-number">04</span>
          <span class="home-card-icon"><i class="fa-solid fa-graduation-cap"></i></span>
        </div>
        <h3>Training, Simulation &amp; Performance Support</h3>
        <p>
          Designing and evaluating simulation-based training, gaze-based training, feedback systems, instructional materials,
          and learning interventions to improve situation awareness, performance, and safety.
        </p>
        <div class="method-tags" aria-label="Methods">
          <span class="method-tag">simulation-based training</span>
          <span class="method-tag">gaze-based training</span>
          <span class="method-tag">situation awareness</span>
          <span class="method-tag">feedback</span>
          <span class="method-tag">instructional design</span>
          <span class="method-tag">performance support</span>
        </div>
      </article>

      <article class="home-card">
        <div class="home-card-top" aria-hidden="true">
          <span class="home-card-number">05</span>
          <span class="home-card-icon"><i class="fa-solid fa-brain"></i></span>
        </div>
        <h3>Statistical Analysis, ML/DL &amp; Generative AI</h3>
        <p>
          Applying statistical analysis, machine learning, deep learning, generative AI, and wearable sensor data to model
          workload, stress, attention, and human performance in complex systems.
        </p>
        <div class="method-tags" aria-label="Methods">
          <span class="method-tag">statistical analysis</span>
          <span class="method-tag">machine learning</span>
          <span class="method-tag">deep learning</span>
          <span class="method-tag">generative AI</span>
          <span class="method-tag">wearable data</span>
          <span class="method-tag">human performance modeling</span>
        </div>
      </article>
    </div>

  </section>
</div>
