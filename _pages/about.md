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

  .home-page .home-section-intro {
    max-width: 860px;
    margin: -0.35rem 0 1.25rem;
    color: var(--global-text-color);
    font-size: 0.98rem;
    line-height: 1.7;
  }

  .home-page .home-section-kicker {
    max-width: 860px;
    margin: -0.75rem 0 0.75rem;
    color: var(--global-text-color-light);
    font-size: 0.95rem;
    line-height: 1.6;
  }

  .home-page .journey-grid {
    position: relative;
    display: grid;
    grid-template-columns: repeat(4, minmax(0, 1fr));
    gap: 1rem;
  }

  .home-page .journey-card {
    position: relative;
    display: flex;
    flex-direction: column;
    min-width: 0;
    height: 100%;
    background: var(--global-card-bg-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    transition:
      transform 160ms ease,
      border-color 160ms ease,
      box-shadow 160ms ease;
  }

  .home-page .journey-card:hover {
    transform: translateY(-2px);
    border-color: var(--global-theme-color);
    box-shadow: 0 0.45rem 1.25rem rgba(0, 0, 0, 0.08);
  }

  .home-page .journey-card:not(:last-child)::after {
    position: absolute;
    top: 5.2rem;
    right: -0.75rem;
    z-index: 2;
    width: 0.9rem;
    height: 0.9rem;
    color: var(--global-theme-color);
    background: var(--global-bg-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    content: ">";
    font-size: 0.52rem;
    font-weight: 900;
    line-height: 0.84rem;
    text-align: center;
  }

  .home-page .journey-image-wrap {
    min-height: 8.7rem;
    overflow: hidden;
    background: var(--global-bg-color);
    border-bottom: 1px solid var(--global-divider-color);
    border-radius: 8px 8px 0 0;
  }

  .home-page .journey-image {
    display: block;
    width: 100%;
    height: 8.7rem;
    object-fit: cover;
  }

  .home-page .journey-content {
    display: flex;
    flex: 1;
    flex-direction: column;
    padding: 1rem;
  }

  .home-page .journey-meta {
    display: flex;
    flex-wrap: wrap;
    gap: 0.35rem;
    margin-bottom: 0.55rem;
    color: var(--global-text-color-light);
    font-size: 0.78rem;
    line-height: 1.35;
  }

  .home-page .journey-theme {
    color: var(--global-theme-color);
    font-weight: 700;
  }

  .home-page .journey-card h3 {
    margin-bottom: 0.35rem;
    color: var(--global-text-color);
    font-size: 0.98rem;
    line-height: 1.35;
    font-weight: 700;
  }

  .home-page .journey-card p {
    margin-bottom: 0.85rem;
    color: var(--global-text-color);
    font-size: 0.9rem;
    line-height: 1.55;
  }

  .home-page .journey-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.35rem;
    margin-top: auto;
  }

  .home-page .journey-tag {
    display: inline-flex;
    align-items: center;
    padding: 0.22rem 0.48rem;
    color: var(--global-text-color);
    background: var(--global-bg-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    font-size: 0.76rem;
    line-height: 1.25;
  }

  .home-page .journey-link {
    align-self: flex-start;
    margin: 0.9rem 0 0;
    padding: 0.34rem 0.62rem;
    color: var(--global-theme-color);
    background: var(--global-bg-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    font-size: 0.8rem;
    line-height: 1.25;
    font-weight: 600;
  }

  .home-page .journey-link:hover {
    color: var(--global-theme-color);
    text-decoration: none;
  }

  .home-page .what-i-do-grid {
    display: grid;
    grid-template-columns: repeat(6, minmax(0, 1fr));
    gap: 1rem;
  }

  .home-page .what-i-do-grid .home-card {
    grid-column: span 2;
    position: relative;
    overflow: hidden;
    --home-card-accent: var(--global-theme-color);
    --home-card-tint: transparent;
    --home-card-badge-bg: var(--global-bg-color);
    --home-card-badge-border: var(--global-divider-color);
    border-top: 3px solid var(--home-card-accent);
    background:
      linear-gradient(180deg, var(--home-card-tint) 0, transparent 4.75rem),
      var(--global-card-bg-color);
    transition:
      transform 160ms ease,
      border-color 160ms ease,
      box-shadow 160ms ease;
  }

  .home-page .what-i-do-grid .home-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 0.45rem 1.25rem rgba(0, 0, 0, 0.08);
  }

  .home-page .what-i-do-grid .home-card:nth-child(1) {
    --home-card-accent: #2f7d87;
    --home-card-tint: rgba(47, 125, 135, 0.08);
    --home-card-badge-bg: rgba(47, 125, 135, 0.1);
    --home-card-badge-border: rgba(47, 125, 135, 0.28);
  }

  .home-page .what-i-do-grid .home-card:nth-child(2) {
    --home-card-accent: #8b5f8e;
    --home-card-tint: rgba(139, 95, 142, 0.08);
    --home-card-badge-bg: rgba(139, 95, 142, 0.1);
    --home-card-badge-border: rgba(139, 95, 142, 0.28);
  }

  .home-page .what-i-do-grid .home-card:nth-child(3) {
    --home-card-accent: #4f8461;
    --home-card-tint: rgba(79, 132, 97, 0.08);
    --home-card-badge-bg: rgba(79, 132, 97, 0.1);
    --home-card-badge-border: rgba(79, 132, 97, 0.28);
  }

  .home-page .what-i-do-grid .home-card:nth-child(4) {
    --home-card-accent: #9a762d;
    --home-card-tint: rgba(154, 118, 45, 0.08);
    --home-card-badge-bg: rgba(154, 118, 45, 0.1);
    --home-card-badge-border: rgba(154, 118, 45, 0.28);
  }

  .home-page .what-i-do-grid .home-card:nth-child(5) {
    --home-card-accent: #526783;
    --home-card-tint: rgba(82, 103, 131, 0.08);
    --home-card-badge-bg: rgba(82, 103, 131, 0.1);
    --home-card-badge-border: rgba(82, 103, 131, 0.28);
  }

  .home-page .what-i-do-grid .home-card .home-card-number,
  .home-page .what-i-do-grid .home-card .home-card-icon {
    color: var(--home-card-accent);
    background: var(--home-card-badge-bg);
    border-color: var(--home-card-badge-border);
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
  html:not([data-theme="dark"]) .home-page .home-section-intro,
  html:not([data-theme="dark"]) .home-page .home-card p,
  html:not([data-theme="dark"]) .home-page .journey-card p,
  html:not([data-theme="dark"]) .home-page .journey-card h3,
  html:not([data-theme="dark"]) .home-page .journey-tag,
  html:not([data-theme="dark"]) .home-page .method-tag {
    color: #333333;
  }

  html:not([data-theme="dark"]) .home-page .home-section-kicker,
  html:not([data-theme="dark"]) .home-page .journey-meta {
    color: #4a4a4a;
  }

  html:not([data-theme="dark"]) .home-page .journey-card {
    background: #fafafa;
    border-color: #dedede;
  }

  html:not([data-theme="dark"]) .home-page .home-card {
    border-color: #dedede;
  }

  html:not([data-theme="dark"]) .home-page .what-i-do-grid .home-card {
    border-top-color: var(--home-card-accent);
  }

  html:not([data-theme="dark"]) .home-page .journey-card:hover {
    box-shadow: 0 0.45rem 1.25rem rgba(0, 0, 0, 0.08);
  }

  html:not([data-theme="dark"]) .home-page .journey-image-wrap {
    background: #f1f1f1;
    border-color: #dedede;
  }

  html:not([data-theme="dark"]) .home-page .home-card-number {
    background: #ffffff;
    border-color: #d6d6d6;
  }

  html:not([data-theme="dark"]) .home-page .home-card-icon {
    background: #ffffff;
    border-color: #d6d6d6;
  }

  html:not([data-theme="dark"]) .home-page .what-i-do-grid .home-card .home-card-number,
  html:not([data-theme="dark"]) .home-page .what-i-do-grid .home-card .home-card-icon {
    color: var(--home-card-accent);
    background: var(--home-card-badge-bg);
    border-color: var(--home-card-badge-border);
  }

  html:not([data-theme="dark"]) .home-page .journey-tag,
  html:not([data-theme="dark"]) .home-page .journey-link,
  html:not([data-theme="dark"]) .home-page .method-tag {
    background: #ffffff;
    border-color: #d8d8d8;
  }

  html:not([data-theme="dark"]) .home-page .journey-link,
  html:not([data-theme="dark"]) .home-page .journey-theme {
    color: #2f5068;
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
    .home-page .journey-grid {
      grid-template-columns: 1fr;
    }

    .home-page .journey-card:not(:last-child)::after {
      top: auto;
      right: 50%;
      bottom: -0.72rem;
      transform: translateX(50%) rotate(90deg);
    }

    .home-page .journey-image,
    .home-page .journey-image-wrap {
      height: 10.5rem;
    }

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
    <h2>Experience Across High-Stakes Human Systems</h2>
    <p class="home-section-kicker">
      From transportation human factors in Springfield, MA to clinical outcomes research in Houston, TX, engineering education
      in Troy, NY, and healthcare systems work in Albany, NY.
    </p>
    <p class="home-section-intro">
      My work spans transportation, healthcare, and engineering education, with a consistent focus on human performance in
      complex, high-stakes systems. Across driving and aviation studies, clinical outcomes research, university teaching, and
      healthcare systems projects, I have applied human factors methods to improve safety, workflow, decision-making, and system
      performance.
    </p>

    <div class="journey-grid">
      <article class="journey-card">
        <div class="journey-image-wrap">
          <img
            class="journey-image"
            src="{{ '/assets/img/projects/atrans/WNEU.JPG' | relative_url }}"
            alt="Western New England University campus associated with ATRANS Lab"
            onerror="this.style.display='none';"
          />
        </div>
        <div class="journey-content">
          <h3>ATRANS Lab</h3>
          <div class="journey-meta">
            <span>Springfield, MA</span>
            <span aria-hidden="true">&middot;</span>
            <span class="journey-theme">Transportation Human Factors</span>
          </div>
          <p>
            My human factors work began at ATRANS Lab, where I worked with Dr. Matthew Romoser on transportation safety studies
            involving teen driver training, aviation simulation, eye tracking, and human performance.
          </p>
          <div class="journey-tags" aria-label="Focus areas">
            <span class="journey-tag">Driving Safety</span>
            <span class="journey-tag">Aviation HF</span>
            <span class="journey-tag">Eye Tracking</span>
            <span class="journey-tag">Simulation</span>
          </div>
          <a
            class="journey-link"
            href="https://wne.edu/engineering/departments/industrial-engineering-and-engineering-management/atrans.cfm"
            target="_blank"
            rel="noopener noreferrer"
          >
            View ATRANS Lab
          </a>
        </div>
      </article>

      <article class="journey-card">
        <div class="journey-image-wrap">
          <img
            class="journey-image"
            src="{{ '/assets/img/projects/houston_methodist/HMH.jpg' | relative_url }}"
            alt="Houston Methodist facility"
            onerror="this.style.display='none';"
          />
        </div>
        <div class="journey-content">
          <h3>Houston Methodist | Center for Outcomes Research</h3>
          <div class="journey-meta">
            <span>Houston, TX</span>
            <span aria-hidden="true">&middot;</span>
            <span class="journey-theme">Clinical Human Factors &amp; Health Systems Research</span>
          </div>
          <p>
            I then moved to Houston, Texas, where I worked as a postdoctoral researcher with Dr. Farzan Sasangohar at Houston
            Methodist&rsquo;s Center for Outcomes Research, applying human factors methods to clinical workflow, clinician workload,
            stress, well-being, and patient safety.
          </p>
          <div class="journey-tags" aria-label="Focus areas">
            <span class="journey-tag">Clinical HF</span>
            <span class="journey-tag">Outcomes Research</span>
            <span class="journey-tag">Wearables</span>
            <span class="journey-tag">Workflow</span>
          </div>
          <a
            class="journey-link"
            href="https://engineering.tamu.edu/industrial/profiles/fsasangohar.html"
            target="_blank"
            rel="noopener noreferrer"
          >
            Mentor Profile
          </a>
        </div>
      </article>

      <article class="journey-card">
        <div class="journey-image-wrap">
          <img
            class="journey-image"
            src="{{ '/assets/img/projects/rpi/RPI.JPG' | relative_url }}"
            alt="Rensselaer Polytechnic Institute campus"
            onerror="this.style.display='none';"
          />
        </div>
        <div class="journey-content">
          <h3>Rensselaer Polytechnic Institute</h3>
          <div class="journey-meta">
            <span>Troy, NY</span>
            <span aria-hidden="true">&middot;</span>
            <span class="journey-theme">Teaching, Research &amp; Engineering Education</span>
          </div>
          <p>
            At RPI, I continued this work through teaching, mentoring, and applied research in human factors, simulation, design
            of experiments, systems engineering, and industrial engineering projects.
          </p>
          <div class="journey-tags" aria-label="Focus areas">
            <span class="journey-tag">Teaching</span>
            <span class="journey-tag">Human Factors</span>
            <span class="journey-tag">Simulation</span>
            <span class="journey-tag">DOE</span>
            <span class="journey-tag">Mentoring</span>
          </div>
        </div>
      </article>

      <article class="journey-card">
        <div class="journey-image-wrap">
          <img
            class="journey-image"
            src="{{ '/assets/img/projects/vascular-access/usgva-simulation-procedure.png' | relative_url }}"
            alt="Clinical workflow and vascular access simulation procedure"
            onerror="this.style.display='none';"
          />
        </div>
        <div class="journey-content">
          <h3>Albany Medical Center</h3>
          <div class="journey-meta">
            <span>Albany, NY</span>
            <span aria-hidden="true">&middot;</span>
            <span class="journey-theme">Healthcare Systems &amp; Clinical Workflow Improvement</span>
          </div>
          <p>
            Through collaborations with Albany Medical Center, I worked on healthcare systems research focused on emergency
            department workflow, vascular access, task analysis, provider performance, and process improvement.
          </p>
          <div class="journey-tags" aria-label="Focus areas">
            <span class="journey-tag">ED Workflow</span>
            <span class="journey-tag">Task Analysis</span>
            <span class="journey-tag">Process Improvement</span>
            <span class="journey-tag">Patient Safety</span>
          </div>
        </div>
      </article>
    </div>

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
