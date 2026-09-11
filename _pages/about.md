---
layout: about
title: Nima Ahmadi, PhD
permalink: /
subtitle: Human Factors Engineer & Researcher
custom_home: true

announcements:
  enabled: false
  scrollable: true
  limit: 1

latest_posts:
  enabled: false
  scrollable: true
  limit: 3

profile:
  align: right
  image: profile.png
  image_circular: false

selected_papers: false
social: true
---

<style>
  .home-page {
    --home-radius: 8px;
    --home-radius-sm: 6px;
    --home-border: rgba(47, 80, 104, 0.18);
    --home-border-strong: rgba(47, 80, 104, 0.28);
    --home-surface: #ffffff;
    --home-surface-soft: #f7f9fa;
    --home-shadow: 0 0.8rem 1.8rem rgba(20, 34, 45, 0.08);
    --home-shadow-hover: 0 1rem 2.2rem rgba(20, 34, 45, 0.11);
    --home-photo-shadow: 0 1.3rem 2.8rem rgba(20, 34, 45, 0.16);
    --home-section-space: 5.25rem;
    color: var(--text-secondary);
  }

  .home-page a {
    transition:
      color 160ms ease,
      border-color 160ms ease,
      background-color 160ms ease,
      box-shadow 160ms ease,
      transform 160ms ease;
  }

  .home-page .home-hero {
    display: grid;
    grid-template-columns: minmax(0, 3fr) minmax(15rem, 2fr);
    gap: 2.6rem;
    align-items: center;
    margin: 0.35rem 0 3.75rem;
    padding: 2.1rem 0 2.85rem;
    border-bottom: 1px solid var(--global-divider-color);
  }

  .home-page .home-hero-content {
    align-self: center;
    max-width: 680px;
  }

  .home-page .home-hero h1 {
    margin-bottom: 0.55rem;
    color: var(--text-primary);
    font-size: 2.9rem;
    line-height: 1.08;
    font-weight: 700;
  }

  .home-page .home-hero .home-role {
    margin-bottom: 1.45rem;
    color: var(--accent);
    font-size: 1.15rem;
    line-height: 1.35;
    font-weight: 650;
  }

  .home-page .home-hero .home-statement {
    max-width: 620px;
    margin-bottom: 1.9rem;
    color: var(--text-secondary);
    font-size: 1rem;
    line-height: 1.68;
    font-weight: 400;
  }

  .home-page .home-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 0.7rem;
  }

  .home-page .home-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 2.75rem;
    padding: 0.72rem 1.08rem;
    color: var(--text-primary);
    background: var(--home-surface);
    border: 1px solid var(--home-border);
    border-radius: var(--home-radius);
    font-size: 0.9rem;
    line-height: 1.3;
    font-weight: 600;
    text-decoration: none;
  }

  .home-page .home-button-primary {
    color: #ffffff;
    background: var(--accent);
    border-color: var(--accent);
  }

  .home-page .home-button:hover {
    transform: translateY(-1px);
    color: var(--global-theme-color);
    border-color: var(--accent);
    text-decoration: none;
    box-shadow: var(--home-shadow);
  }

  .home-page .home-button-primary:hover {
    color: #ffffff;
    background: var(--global-theme-color);
  }

  .home-page .home-hero-portrait {
    align-self: center;
    justify-self: end;
    width: min(100%, 21rem);
    max-height: 580px;
    padding: 0.42rem;
    background: var(--home-surface);
    border: 1px solid var(--home-border);
    border-radius: var(--home-radius);
    box-shadow: var(--home-photo-shadow);
  }

  .home-page .home-hero-portrait img {
    display: block;
    width: 100%;
    height: min(52vh, 560px);
    min-height: 390px;
    aspect-ratio: 4 / 5;
    object-fit: cover;
    object-position: center top;
    border-radius: var(--home-radius-sm);
  }

  .home-page .home-section {
    margin-bottom: var(--home-section-space);
  }

  .home-page .home-section h2 {
    margin-bottom: 1rem;
    color: var(--text-primary);
    font-size: 1.58rem;
    line-height: 1.2;
    font-weight: 650;
  }

  .home-page .home-section-intro {
    max-width: 780px;
    margin: -0.15rem 0 1.55rem;
    color: var(--text-secondary);
    font-size: 0.96rem;
    line-height: 1.68;
    font-weight: 400;
  }

  .home-page .home-section-kicker {
    max-width: 760px;
    margin: -0.45rem 0 0.75rem;
    color: var(--text-muted);
    font-size: 0.9rem;
    line-height: 1.58;
    font-weight: 500;
  }

  .home-page .journey-section {
    padding: 0;
    border: 0;
  }

  .home-page .journey-grid {
    position: relative;
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.5rem;
    margin-top: 1.9rem;
    align-items: stretch;
  }

  .home-page .journey-card {
    position: relative;
    display: flex;
    flex-direction: column;
    min-width: 0;
    height: 100%;
    overflow: hidden;
    background: var(--home-surface);
    border: 1px solid var(--home-border);
    border-radius: var(--home-radius);
    box-shadow: 0 0.35rem 1rem rgba(20, 34, 45, 0.04);
    transition:
      transform 160ms ease,
      border-color 160ms ease,
      box-shadow 160ms ease;
  }

  .home-page .journey-card:hover {
    transform: translateY(-1px);
    border-color: var(--home-border-strong);
    box-shadow: var(--home-shadow-hover);
  }

  .home-page .journey-card::after {
    display: none;
  }

  .home-page .journey-image-wrap {
    aspect-ratio: 16 / 9;
    min-height: 0;
    overflow: hidden;
    background: var(--home-surface-soft);
    border-bottom: 1px solid var(--home-border);
  }

  .home-page .journey-image {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
  }

  .home-page .journey-content {
    display: grid;
    flex: 1;
    grid-template-rows: auto auto auto minmax(6.15rem, auto) auto;
    padding: 1.2rem 1.2rem 1.15rem;
  }

  .home-page .journey-meta {
    display: grid;
    gap: 0.28rem;
    min-height: 3.25rem;
    margin-bottom: 0.9rem;
    color: var(--text-muted);
    font-size: 0.84rem;
    line-height: 1.4;
    font-weight: 500;
  }

  .home-page .journey-years {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: fit-content;
    margin-bottom: 0.78rem;
    padding: 0.28rem 0.56rem;
    color: var(--accent);
    background: var(--accent-soft);
    border: 1px solid transparent;
    border-radius: 999px;
    font-size: 0.76rem;
    line-height: 1.25;
    font-weight: 650;
  }

  .home-page .journey-theme {
    color: var(--accent);
    font-weight: 700;
  }

  .home-page .journey-focus-label {
    color: var(--text-primary);
    font-weight: 700;
  }

  .home-page .journey-card h3 {
    min-height: 2.85rem;
    margin-bottom: 0.45rem;
    color: var(--text-primary);
    font-size: 1.05rem;
    line-height: 1.35;
    font-weight: 650;
  }

  .home-page .journey-card h3.journey-title-long {
    font-size: 1rem;
  }

  .home-page .journey-affiliation {
    display: grid;
    gap: 0.14rem;
    min-height: 2.45rem;
    margin: 0 0 0.65rem;
    color: var(--text-secondary);
    font-size: 0.85rem;
    line-height: 1.42;
    font-weight: 500;
  }

  .home-page .journey-affiliation span:first-child {
    font-weight: 700;
  }

  .home-page .journey-card p {
    margin-bottom: 0;
    color: var(--text-secondary);
    font-size: 0.93rem;
    line-height: 1.64;
    font-weight: 400;
  }

  .home-page .journey-footer {
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    min-height: 4.9rem;
    margin-top: 1.05rem;
  }

  .home-page .journey-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.38rem;
    margin-top: 0;
  }

  .home-page .journey-tag {
    display: inline-flex;
    align-items: center;
    padding: 0.25rem 0.54rem;
    color: var(--text-secondary);
    background: var(--home-surface-soft);
    border: 1px solid var(--home-border);
    border-radius: 999px;
    font-size: 0.76rem;
    line-height: 1.25;
    font-weight: 500;
  }

  .home-page .journey-link {
    align-self: flex-start;
    margin: 1rem 0 0;
    padding: 0.38rem 0.68rem;
    color: var(--accent);
    background: transparent;
    border: 1px solid var(--home-border);
    border-radius: 999px;
    font-size: 0.8rem;
    line-height: 1.3;
    font-weight: 600;
  }

  .home-page .journey-link-spacer {
    display: block;
    height: 2.08rem;
    margin-top: 1rem;
  }

  .home-page .journey-link:hover {
    color: var(--global-theme-color);
    border-color: var(--home-border-strong);
    text-decoration: none;
  }

  .home-page .what-i-do-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.5rem;
    align-items: stretch;
  }

  .home-page .what-i-do-grid .home-card {
    position: relative;
    overflow: hidden;
    --home-card-accent: var(--global-theme-color);
    --home-card-badge-bg: var(--home-surface-soft);
    --home-card-badge-border: var(--home-border);
    border-top: 2px solid var(--home-card-accent);
    background: var(--home-surface);
    box-shadow: 0 0.35rem 1rem rgba(20, 34, 45, 0.04);
    transition:
      transform 160ms ease,
      border-color 160ms ease,
      box-shadow 160ms ease;
  }

  .home-page .what-i-do-grid .home-card:hover {
    transform: translateY(-1px);
    border-color: var(--home-border-strong);
    box-shadow: var(--home-shadow-hover);
  }

  .home-page .what-i-do-grid .home-card:nth-child(1) {
    --home-card-accent: #2f7d87;
    --home-card-badge-bg: rgba(47, 125, 135, 0.1);
    --home-card-badge-border: rgba(47, 125, 135, 0.28);
  }

  .home-page .what-i-do-grid .home-card:nth-child(2) {
    --home-card-accent: #8b5f8e;
    --home-card-badge-bg: rgba(139, 95, 142, 0.1);
    --home-card-badge-border: rgba(139, 95, 142, 0.28);
  }

  .home-page .what-i-do-grid .home-card:nth-child(3) {
    --home-card-accent: #4f8461;
    --home-card-badge-bg: rgba(79, 132, 97, 0.1);
    --home-card-badge-border: rgba(79, 132, 97, 0.28);
  }

  .home-page .what-i-do-grid .home-card:nth-child(4) {
    --home-card-accent: #9a762d;
    --home-card-badge-bg: rgba(154, 118, 45, 0.1);
    --home-card-badge-border: rgba(154, 118, 45, 0.28);
  }

  .home-page .what-i-do-grid .home-card:nth-child(5) {
    --home-card-accent: #526783;
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
    min-height: 18rem;
    padding: 1.45rem;
    background: var(--home-surface);
    border: 1px solid var(--home-border);
    border-radius: var(--home-radius);
  }

  .home-page .home-card-number {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 2rem;
    height: 2rem;
    margin-bottom: 0.9rem;
    color: var(--accent);
    border: 1px solid var(--home-border);
    border-radius: 999px;
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0;
  }

  .home-page .home-card-top {
    display: flex;
    align-items: center;
    gap: 0.62rem;
    min-height: 2.25rem;
    margin-bottom: 0.95rem;
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
    color: var(--accent);
    background: var(--home-surface-soft);
    border: 1px solid var(--home-border);
    border-radius: 999px;
    font-size: 0.85rem;
  }

  .home-page .home-card h3 {
    min-height: 2.85rem;
    margin-bottom: 0.72rem;
    color: var(--text-primary);
    font-size: 1.05rem;
    line-height: 1.35;
    font-weight: 650;
  }

  .home-page .home-card p {
    min-height: 6.2rem;
    margin-bottom: 1.05rem;
    color: var(--text-secondary);
    font-size: 0.93rem;
    line-height: 1.66;
    font-weight: 400;
  }

  .home-page .method-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.42rem;
    margin-top: 0.85rem;
  }

  .home-page .home-card .method-tags {
    margin-top: auto;
    padding-top: 0.1rem;
  }

  .home-page .method-tag {
    display: inline-flex;
    align-items: center;
    padding: 0.25rem 0.54rem;
    color: var(--text-secondary);
    background: var(--home-surface-soft);
    border: 1px solid var(--home-border);
    border-radius: 999px;
    font-size: 0.76rem;
    line-height: 1.25;
    font-weight: 500;
  }

  .home-page .teaching-teaser {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 1.25rem;
    padding: 1.35rem 1.45rem;
    background: var(--home-surface);
    border: 1px solid var(--home-border);
    border-radius: var(--home-radius);
    box-shadow: 0 0.35rem 1rem rgba(20, 34, 45, 0.04);
  }

  .home-page .teaching-teaser p {
    max-width: 720px;
    margin: 0;
    color: var(--text-primary);
    font-size: 0.96rem;
    line-height: 1.6;
    font-weight: 400;
  }

  .post article > .social {
    margin-top: 0.75rem;
    padding-top: 1.75rem;
    border-top: 1px solid var(--global-divider-color);
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
  html:not([data-theme="dark"]) .home-page .journey-affiliation,
  html:not([data-theme="dark"]) .home-page .journey-tag,
  html:not([data-theme="dark"]) .home-page .method-tag {
    color: #333333;
  }

  html:not([data-theme="dark"]) .home-page .home-button-primary {
    color: #ffffff;
  }

  html:not([data-theme="dark"]) .home-page .home-section-kicker,
  html:not([data-theme="dark"]) .home-page .journey-meta {
    color: #5b6268;
  }

  html:not([data-theme="dark"]) .home-page .journey-theme {
    color: #2f5068;
  }

  html[data-theme="dark"] .home-page {
    --home-border: rgba(143, 206, 225, 0.18);
    --home-border-strong: rgba(143, 206, 225, 0.32);
    --home-surface: #24282d;
    --home-surface-soft: #1f2328;
    --home-shadow: 0 0.8rem 1.8rem rgba(0, 0, 0, 0.18);
    --home-shadow-hover: 0 1rem 2.2rem rgba(0, 0, 0, 0.24);
    --home-photo-shadow: 0 1.3rem 2.8rem rgba(0, 0, 0, 0.3);
  }

  html[data-theme="dark"] .home-page .home-button-primary {
    color: #101417;
  }

  html[data-theme="dark"] .home-page .home-button-primary:hover {
    color: #101417;
  }

  html[data-theme="dark"] .home-page .what-i-do-grid .home-card:nth-child(4) {
    --home-card-accent: #d2aa55;
    --home-card-badge-bg: rgba(210, 170, 85, 0.14);
    --home-card-badge-border: rgba(210, 170, 85, 0.28);
  }

  html[data-theme="dark"] .home-page .journey-tag,
  html[data-theme="dark"] .home-page .method-tag {
    color: var(--text-muted);
  }

  @media (max-width: 900px) {
    .home-page {
      --home-section-space: 4rem;
    }

    .home-page .home-hero {
      grid-template-columns: 1fr;
      gap: 1.8rem;
      margin-bottom: 3.5rem;
      padding: 1.85rem 0 2.65rem;
    }

    .home-page .home-hero-portrait {
      justify-self: start;
      width: min(100%, 18rem);
      max-height: none;
    }

    .home-page .home-hero-portrait img {
      height: auto;
      min-height: 0;
    }

    .home-page .journey-grid {
      grid-template-columns: 1fr;
    }

    .home-page .home-hero h1 {
      font-size: 2.3rem;
    }
  }

  @media (max-width: 760px) {
    .home-page .what-i-do-grid {
      grid-template-columns: 1fr;
    }

    .home-page .what-i-do-grid .home-card {
      grid-column: auto;
    }
  }

  @media (max-width: 575px) {
    .home-page {
      --home-section-space: 3.4rem;
    }

    .home-page .home-hero {
      gap: 1.35rem;
      margin-top: 0.1rem;
      margin-bottom: 3rem;
      padding: 1.15rem 0 2.25rem;
    }

    .home-page .home-hero h1 {
      font-size: 2.05rem;
    }

    .home-page .home-hero .home-role {
      font-size: 1.02rem;
    }

    .home-page .home-actions {
      flex-direction: column;
    }

    .home-page .home-button {
      width: 100%;
    }

    .home-page .home-card,
    .home-page .journey-content {
      padding: 1.1rem;
    }

    .home-page .journey-content {
      grid-template-rows: auto;
    }

    .home-page .journey-card h3,
    .home-page .journey-affiliation,
    .home-page .journey-meta,
    .home-page .home-card h3,
    .home-page .home-card p {
      min-height: 0;
    }

    .home-page .journey-footer {
      min-height: 0;
    }

    .home-page .teaching-teaser {
      align-items: flex-start;
      flex-direction: column;
      padding: 1.1rem;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    .home-page a,
    .home-page .home-button,
    .home-page .journey-card,
    .home-page .home-card {
      transition: none;
    }

    .home-page .home-button:hover,
    .home-page .journey-card:hover,
    .home-page .what-i-do-grid .home-card:hover {
      transform: none;
    }
  }
</style>

<div class="home-page">
  <section class="home-hero">
    <div class="home-hero-content">
      <h1>Nima Ahmadi, PhD</h1>
      <p class="home-role">Human Factors Engineer &amp; Researcher</p>
      <p class="home-statement">
        I study how people interact with complex healthcare, aviation, and safety-critical systems. My work combines human
        factors methods, experimental design, multimodal sensing, statistical analysis, and AI-enabled modeling to support safer
        and more usable technologies.
      </p>
      <div class="home-actions" aria-label="Portfolio links">
        <a class="home-button home-button-primary" href="{{ '/projects/' | relative_url }}">View Projects</a>
        <a class="home-button" href="{{ '/cv/' | relative_url }}">View CV</a>
        <a class="home-button" href="{{ '/contact/' | relative_url }}">Contact Me</a>
      </div>
    </div>
    <div class="home-hero-portrait">
      <img
        src="{{ '/assets/img/profile.png' | relative_url }}"
        width="1122"
        height="1402"
        alt="Portrait of Nima Ahmadi"
        loading="eager"
        decoding="async"
      />
    </div>
  </section>

  <section class="home-section journey-section">
    <h2>Experience Across High-Stakes Human Systems</h2>
    <p class="home-section-kicker">
      From transportation human factors in Springfield, MA to clinical outcomes research in Houston, TX, engineering education
      in Troy, NY, and healthcare systems work in Albany, NY.
    </p>
    <p class="home-section-intro">
      My work spans transportation, healthcare, and engineering education, with a consistent focus on human performance,
      workflow, decision-making, and safety in complex systems.
    </p>

    <div class="journey-grid">
      <article class="journey-card">
        <div class="journey-image-wrap">
          <img
            class="journey-image"
            src="{{ '/assets/img/projects/atrans/WNEU.JPG' | relative_url }}"
            width="4032"
            height="3024"
            alt="Western New England University campus associated with ATRANS"
            loading="lazy"
            decoding="async"
            onerror="this.style.display='none';"
          />
        </div>
        <div class="journey-content">
          <h3 class="journey-title-long">Center for Advanced Training Research and Naturalistic Studies (ATRANS)</h3>
          <div class="journey-affiliation" aria-label="Institution and department">
            <span>Western New England University</span>
            <span>Department of Industrial Engineering and Engineering Management</span>
          </div>
          <span class="journey-years">2015&ndash;2020</span>
          <div class="journey-meta">
            <div class="journey-location">Springfield, MA</div>
            <div class="journey-focus">
              <span class="journey-focus-label">Focus:</span>
              <span class="journey-theme">Transportation Human Factors</span>
            </div>
          </div>
          <p>
            Worked with Dr. Matthew Romoser on transportation safety studies involving teen driver training, aviation simulation,
            eye tracking, and human performance.
          </p>
          <div class="journey-footer">
            <div class="journey-tags" aria-label="Focus areas">
              <span class="journey-tag">Driving Safety</span>
              <span class="journey-tag">Aviation HF</span>
              <span class="journey-tag">Simulation</span>
            </div>
            <a
              class="journey-link"
              href="https://wne.edu/engineering/departments/industrial-engineering-and-engineering-management/atrans.cfm"
              target="_blank"
              rel="noopener noreferrer"
            >
              View ATRANS
            </a>
          </div>
        </div>
      </article>

      <article class="journey-card">
        <div class="journey-image-wrap">
          <img
            class="journey-image"
            src="{{ '/assets/img/projects/houston_methodist/HMH.jpg' | relative_url }}"
            width="4608"
            height="3072"
            alt="Houston Methodist facility"
            loading="lazy"
            decoding="async"
            onerror="this.style.display='none';"
          />
        </div>
        <div class="journey-content">
          <h3>Houston Methodist Hospital</h3>
          <div class="journey-affiliation" aria-label="Center">
            <span>Center for Outcomes Research</span>
          </div>
          <span class="journey-years">2020&ndash;2022</span>
          <div class="journey-meta">
            <div class="journey-location">Houston, TX</div>
            <div class="journey-focus">
              <span class="journey-focus-label">Focus:</span>
              <span class="journey-theme">Clinical Human Factors &amp; Health Systems Research</span>
            </div>
          </div>
          <p>
            Worked as a postdoctoral researcher with Dr. Farzan Sasangohar, applying human factors methods to clinical workflow,
            clinician workload, stress, well-being, and patient safety.
          </p>
          <div class="journey-footer">
            <div class="journey-tags" aria-label="Focus areas">
              <span class="journey-tag">Clinical HF</span>
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
        </div>
      </article>

      <article class="journey-card">
        <div class="journey-image-wrap">
          <img
            class="journey-image"
            src="{{ '/assets/img/projects/rpi/RPI.JPG' | relative_url }}"
            width="4032"
            height="3024"
            alt="Rensselaer Polytechnic Institute campus"
            loading="lazy"
            decoding="async"
            onerror="this.style.display='none';"
          />
        </div>
        <div class="journey-content">
          <h3>Rensselaer Polytechnic Institute (RPI)</h3>
          <div class="journey-affiliation" aria-label="Department">
            <span>Department of Industrial and Systems Engineering</span>
          </div>
          <span class="journey-years">2022&ndash;Present</span>
          <div class="journey-meta">
            <div class="journey-location">Troy, NY</div>
            <div class="journey-focus">
              <span class="journey-focus-label">Focus:</span>
              <span class="journey-theme">Teaching, Research &amp; Engineering Education</span>
            </div>
          </div>
          <p>
            Continued teaching, mentoring, and applied research in human factors, simulation, design of experiments, systems
            engineering, and industrial engineering projects.
          </p>
          <div class="journey-footer">
            <div class="journey-tags" aria-label="Focus areas">
              <span class="journey-tag">Teaching</span>
              <span class="journey-tag">Human Factors</span>
              <span class="journey-tag">DOE</span>
            </div>
            <span class="journey-link-spacer" aria-hidden="true"></span>
          </div>
        </div>
      </article>

      <article class="journey-card">
        <div class="journey-image-wrap">
          <img
            class="journey-image"
            src="{{ '/assets/img/emergency.jpg' | relative_url }}"
            width="4928"
            height="3264"
            alt="Clinical workflow and vascular access simulation procedure"
            loading="lazy"
            decoding="async"
            onerror="this.style.display='none';"
          />
        </div>
        <div class="journey-content">
          <h3>Albany Medical Center</h3>
          <div class="journey-affiliation" aria-label="Collaboration">
            <span>Emergency Department Research Collaboration</span>
          </div>
          <span class="journey-years">2023&ndash;Present</span>
          <div class="journey-meta">
            <div class="journey-location">Albany, NY</div>
            <div class="journey-focus">
              <span class="journey-focus-label">Focus:</span>
              <span class="journey-theme">Healthcare Systems &amp; Clinical Workflow Improvement</span>
            </div>
          </div>
          <p>
            Collaborated on healthcare systems research focused on emergency department workflow, vascular access, task analysis,
            provider performance, and process improvement.
          </p>
          <div class="journey-footer">
            <div class="journey-tags" aria-label="Focus areas">
              <span class="journey-tag">ED Workflow</span>
              <span class="journey-tag">Task Analysis</span>
              <span class="journey-tag">Patient Safety</span>
            </div>
            <span class="journey-link-spacer" aria-hidden="true"></span>
          </div>
        </div>
      </article>
    </div>

  </section>

  <section class="home-section">
    <h2>Core Expertise</h2>
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
          <span class="method-tag">simulation studies</span>
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
          <span class="method-tag">generative AI</span>
          <span class="method-tag">human performance modeling</span>
        </div>
      </article>
    </div>

  </section>

  <section class="home-section">
    <h2>Teaching Portfolio</h2>
    <div class="teaching-teaser">
      <p>
        Courses span human factors, engineering design, healthcare and manufacturing simulation, analytics, systems engineering,
        and computing.
      </p>
      <a class="home-button" href="{{ '/teaching/' | relative_url }}">View Teaching Portfolio &rarr;</a>
    </div>
  </section>
</div>
