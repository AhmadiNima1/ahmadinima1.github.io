---
layout: page
title: Selected Projects
permalink: /projects/
nav: false
nav_order: 2
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400..700&display=swap" rel="stylesheet">

<style>
  .post-title,
  .page-title,
  .post h1 {
    font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    font-weight: 700;
    letter-spacing: 0;
  }

  .projects {
    --projects-font: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    --project-accent-default: #2f5068;
    --project-accent-driver: #233f63;
    --project-accent-aviation: #2f6f9f;
    --project-accent-teal: #2e7d78;
    --project-accent-mental-health: #7a5f92;
    --project-accent-outpatient: #9a6b2f;
    --project-accent-navigation: #6873b4;
    font-family: var(--projects-font);
  }

  html[data-theme="dark"] .projects {
    --project-accent-driver: #7fa4d2;
    --project-accent-aviation: #72a9cf;
    --project-accent-teal: #70b8b2;
    --project-accent-mental-health: #b49ad0;
    --project-accent-outpatient: #d4a15b;
    --project-accent-navigation: #a3ade6;
  }

  .projects a,
  .projects button,
  .projects .card,
  .projects .project-overview-card {
    font-family: inherit;
  }

  html:not([data-theme="dark"]) .projects .card,
  html:not([data-theme="dark"]) .projects .card .card-body,
  html:not([data-theme="dark"]) .project-card,
  html:not([data-theme="dark"]) .archive__item,
  html:not([data-theme="dark"]) .page__content {
    color: #333333 !important;
  }

  html:not([data-theme="dark"]) .projects .card .card-title,
  html:not([data-theme="dark"]) .projects .card h5,
  html:not([data-theme="dark"]) .projects .card h6,
  html:not([data-theme="dark"]) .projects .card .card-body p,
  html:not([data-theme="dark"]) .projects .card .card-body .card-text,
  html:not([data-theme="dark"]) .projects .card .card-body .card-text strong,
  html:not([data-theme="dark"]) .projects .card .skills,
  html:not([data-theme="dark"]) .projects .card .skills *,
  html:not([data-theme="dark"]) .projects .card .tags,
  html:not([data-theme="dark"]) .projects .card .tags *,
  html:not([data-theme="dark"]) .projects .card .project-tags,
  html:not([data-theme="dark"]) .projects .card .project-tags *,
  html:not([data-theme="dark"]) .project-card p,
  html:not([data-theme="dark"]) .project-card .card-text,
  html:not([data-theme="dark"]) .archive__item-excerpt {
    color: #333333 !important;
  }

  html:not([data-theme="dark"]) .projects .card .caption {
    color: #444444 !important;
  }

  html[data-theme="dark"] .projects .card .card-body .card-text {
    color: #e0e0e0 !important;
  }

  html[data-theme="dark"] .projects .card .card-body .card-text strong,
  html[data-theme="dark"] .projects .card .card-title {
    color: #ffffff !important;
  }

  html[data-theme="dark"] .projects .card .caption {
    color: #d8dee9 !important;
  }

  .projects .project-header {
    padding: 1.2rem 1.25rem 0.95rem;
  }

  .projects .project-category {
    display: inline-flex;
    gap: 0.4rem;
    align-items: center;
    margin-bottom: 0.45rem;
    color: var(--project-accent, var(--text-muted));
    font-size: 0.78rem;
    font-weight: 650;
    line-height: 1.3;
    text-transform: uppercase;
    letter-spacing: 0.035em;
  }

  .projects .project-category i {
    color: var(--project-accent, var(--accent));
    font-size: 0.9rem;
  }

  .projects .project-index {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-width: 1.8rem;
    padding: 0.14rem 0.42rem;
    color: var(--project-accent, var(--accent));
    background: var(--page-bg);
    border: 1px solid var(--project-accent, var(--border));
    border-radius: 999px;
    font-size: 0.72rem;
    line-height: 1.2;
    font-weight: 650;
  }

  .projects .project-header .card-title {
    margin-bottom: 0;
    color: var(--text-primary);
    font-size: 1.12rem;
    line-height: 1.34;
    font-weight: 650;
  }

  .projects > .card {
    overflow: hidden;
    background: var(--card-bg);
    border: 1px solid var(--border);
    border-left: 4px solid var(--project-accent, var(--accent));
    border-radius: 8px;
    transition:
      transform 160ms ease,
      border-color 160ms ease,
      box-shadow 160ms ease;
  }

  .projects > .card:hover {
    transform: translateY(-2px);
    border-color: var(--border);
    border-left-color: var(--project-accent, var(--accent));
    box-shadow: 0 0.45rem 1.25rem rgba(0, 0, 0, 0.08);
  }

  html[data-theme="light"] .projects > .card {
    border-left-color: var(--project-accent, var(--project-accent-default));
  }

  .projects > .card#driving-safety {
    --project-accent: var(--project-accent-driver);
  }

  .projects > .card#aviation-human-factors,
  .projects > .card#pilot-performance-vocal-stress {
    --project-accent: var(--project-accent-aviation);
  }

  .projects > .card#clinician-stress-workload,
  .projects > .card#vascular-access-workflow {
    --project-accent: var(--project-accent-teal);
  }

  .projects > .card#healthcare-worker-mental-health {
    --project-accent: var(--project-accent-mental-health);
  }

  .projects > .card#outpatient-compliance-live-chat {
    --project-accent: var(--project-accent-outpatient);
  }

  .projects > .card#digital-health-usability {
    --project-accent: var(--project-accent-navigation);
  }

  .projects > .card .card-img-top {
    border-top: 1px solid var(--border);
    border-bottom: 1px solid var(--border);
  }

  .projects .project-subsection {
    margin: 1.25rem 0;
    padding: 1rem;
    color: var(--text-secondary);
    background: var(--card-bg);
    border: 1px solid var(--border);
    border-radius: 8px;
  }

  .projects .project-subsection-label {
    display: inline-flex;
    gap: 0.4rem;
    align-items: center;
    margin-bottom: 0.45rem;
    color: var(--text-muted);
    font-size: 0.78rem;
    font-weight: 650;
    line-height: 1.3;
    text-transform: uppercase;
    letter-spacing: 0.035em;
  }

  .projects .project-subsection-label i {
    color: var(--project-accent, var(--accent));
    font-size: 0.9rem;
  }

  .projects .project-subsection h6 {
    margin-bottom: 0.65rem;
    color: var(--text-primary);
    font-size: 1.05rem;
    line-height: 1.35;
    font-weight: 650;
  }

  .projects .project-subsection .card-text {
    margin-bottom: 0;
  }

  .projects .card-body .card-text {
    font-size: 0.93rem;
    line-height: 1.64;
    font-weight: 400;
  }

  .projects .project-detail-heading {
    margin: 1rem 0 0.45rem;
    color: #252a31;
    font-size: 0.9rem;
    line-height: 1.35;
    font-weight: 600;
    letter-spacing: 0.02em;
    text-transform: uppercase;
  }

  html[data-theme="dark"] .projects .project-detail-heading {
    color: #f1f5f9;
  }

  .projects .project-detail-list {
    margin: 0 0 0.95rem 1.1rem;
    padding: 0;
    color: var(--text-secondary);
    font-size: 0.94rem;
    line-height: 1.6;
  }

  .projects .project-detail-list li {
    margin-bottom: 0.3rem;
  }

  .projects .project-method-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
    margin-bottom: 0.95rem;
  }

  html:not([data-theme="dark"]) .projects .project-category {
    color: var(--project-accent, #555555) !important;
  }

  html:not([data-theme="dark"]) .projects .project-header .card-title {
    color: #222222 !important;
  }

  html:not([data-theme="dark"]) .projects .project-subsection {
    color: #333333 !important;
    background: #fafafa;
    border-color: #dedede;
  }

  html:not([data-theme="dark"]) .projects .project-subsection-label {
    color: #555555 !important;
  }

  html:not([data-theme="dark"]) .projects .project-subsection h6,
  html:not([data-theme="dark"]) .projects .project-subsection .card-text,
  html:not([data-theme="dark"]) .projects .project-detail-list {
    color: #333333 !important;
  }

  html:not([data-theme="dark"]) .projects .project-detail-heading {
    color: #252a31 !important;
  }

  .projects .project-overview {
    margin-bottom: 2rem;
  }

  .projects .project-carousel-shell {
    position: relative;
    --carousel-control-size: 2.35rem;
    --carousel-control-offset: calc((var(--carousel-control-size) + 0.65rem) * -1);
  }

  .projects .project-carousel-controls {
    position: absolute;
    inset: 0;
    z-index: 2;
    pointer-events: none;
  }

  .projects .project-carousel-control {
    position: absolute;
    top: 50%;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: var(--carousel-control-size);
    height: var(--carousel-control-size);
    color: var(--accent);
    background: var(--card-bg);
    border: 1px solid var(--accent);
    border-radius: 999px;
    box-shadow: 0 0.35rem 1rem rgba(20, 34, 45, 0.08);
    cursor: pointer;
    pointer-events: auto;
    transform: translateY(-50%);
    text-decoration: none;
    transition:
      color 160ms ease,
      border-color 160ms ease,
      background-color 160ms ease,
      opacity 160ms ease,
      box-shadow 160ms ease;
  }

  .projects .project-carousel-control[data-carousel-direction="prev"] {
    left: var(--carousel-control-offset);
  }

  .projects .project-carousel-control[data-carousel-direction="next"] {
    right: var(--carousel-control-offset);
  }

  .projects .project-carousel-control:hover:not(:disabled) {
    color: var(--page-bg);
    background: var(--accent);
    border-color: var(--accent);
    box-shadow: 0 0.55rem 1.25rem rgba(20, 34, 45, 0.12);
    text-decoration: none;
  }

  .projects .project-carousel-control:disabled {
    opacity: 0.34;
    cursor: default;
    color: var(--text-secondary);
    border-color: var(--border);
    box-shadow: none;
  }

  .projects .project-overview h2 {
    margin-bottom: 0.45rem;
    color: var(--text-primary);
    font-size: 1.52rem;
    line-height: 1.24;
    font-weight: 700;
  }

  .projects .project-overview-intro {
    max-width: 860px;
    margin-bottom: 0.55rem;
    color: var(--text-secondary);
    font-size: 0.96rem;
    line-height: 1.68;
    font-weight: 400;
  }

  .projects .project-overview-note,
  .projects .project-case-studies-intro {
    max-width: 860px;
    margin: 0 0 1.25rem;
    color: var(--text-muted);
    font-size: 0.92rem;
    line-height: 1.6;
    font-weight: 500;
  }

  .projects .project-case-studies {
    margin: 2.35rem 0 1.2rem;
    padding-top: 1.55rem;
    border-top: 1px solid var(--border);
  }

  .projects .project-case-studies h2 {
    margin-bottom: 0.45rem;
    color: var(--text-primary);
    font-size: 1.48rem;
    line-height: 1.25;
    font-weight: 700;
  }

  .projects .project-overview-grid {
    display: grid;
    grid-auto-columns: calc((100% - 1.2rem) / 2);
    grid-auto-flow: column;
    grid-template-columns: none;
    gap: 1.2rem;
    align-items: stretch;
    overflow-x: auto;
    overscroll-behavior-x: contain;
    padding: 0.15rem 0.1rem 0.9rem;
    scroll-padding-inline: 0.1rem;
    scroll-behavior: smooth;
    scroll-snap-type: x mandatory;
    -webkit-overflow-scrolling: touch;
  }

  .projects .project-overview-grid::-webkit-scrollbar {
    height: 0.58rem;
  }

  .projects .project-overview-grid::-webkit-scrollbar-track {
    background: transparent;
  }

  .projects .project-overview-grid::-webkit-scrollbar-thumb {
    background: var(--border);
    border-radius: 999px;
  }

  .projects .project-overview-card {
    --project-accent: var(--project-accent-default);
    display: flex;
    flex-direction: column;
    min-width: 0;
    height: 100%;
    min-height: 34.5rem;
    overflow: hidden;
    color: var(--text-secondary);
    background: var(--card-bg);
    border: 1px solid var(--border);
    border-top: 3px solid var(--project-accent);
    border-radius: 8px;
    scroll-snap-align: start;
    scroll-snap-stop: always;
    transition:
      transform 160ms ease,
      border-color 160ms ease,
      box-shadow 160ms ease;
  }

  .projects .project-overview-card:nth-child(1) {
    --project-accent: var(--project-accent-driver);
  }

  .projects .project-overview-card:nth-child(2),
  .projects .project-overview-card:nth-child(3) {
    --project-accent: var(--project-accent-aviation);
  }

  .projects .project-overview-card:nth-child(4),
  .projects .project-overview-card:nth-child(6) {
    --project-accent: var(--project-accent-teal);
  }

  .projects .project-overview-card:nth-child(5) {
    --project-accent: var(--project-accent-mental-health);
  }

  .projects .project-overview-card:nth-child(7) {
    --project-accent: var(--project-accent-outpatient);
  }

  .projects .project-overview-card:nth-child(8) {
    --project-accent: var(--project-accent-navigation);
  }

  .projects .project-overview-card:hover {
    transform: translateY(-2px);
    border-color: var(--border);
    border-top-color: var(--project-accent);
    box-shadow: 0 0.45rem 1.25rem rgba(0, 0, 0, 0.08);
  }

  .projects .project-overview-image-wrap {
    aspect-ratio: 16 / 9;
    min-height: 0;
    overflow: hidden;
    background: var(--page-bg);
    border-bottom: 1px solid var(--border);
  }

  .projects .project-overview-placeholder,
  .projects .project-detail-placeholder {
    display: flex;
    width: 100%;
    height: 100%;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 0.45rem;
    padding: 1rem;
    color: var(--text-secondary);
    background:
      linear-gradient(135deg, rgba(47, 80, 104, 0.14), rgba(47, 80, 104, 0.04)),
      var(--page-bg);
    text-align: center;
  }

  .projects .project-detail-placeholder {
    height: 320px;
    border-top: 1px solid var(--border);
    border-bottom: 1px solid var(--border);
  }

  .projects .project-overview-placeholder i,
  .projects .project-detail-placeholder i {
    color: var(--accent);
    font-size: 1.6rem;
  }

  .projects .project-overview-placeholder span,
  .projects .project-detail-placeholder span {
    max-width: 18rem;
    color: var(--text-primary);
    font-size: 0.88rem;
    line-height: 1.35;
    font-weight: 650;
  }

  .projects .project-overview-image {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  .projects .project-overview-content {
    display: grid;
    flex: 1;
    grid-template-rows: minmax(2.6rem, auto) minmax(4.2rem, auto) minmax(5.6rem, auto) auto auto;
    padding: 1.1rem;
  }

  .projects .project-overview-label {
    display: inline-flex;
    align-items: center;
    gap: 0.45rem;
    min-height: 2.6rem;
    margin-bottom: 0.45rem;
    color: var(--project-accent);
    font-size: 0.78rem;
    line-height: 1.3;
    font-weight: 650;
    letter-spacing: 0.035em;
    text-transform: uppercase;
  }

  .projects .project-overview-card h3 {
    min-height: 4.2rem;
    margin-bottom: 0.55rem;
    color: var(--text-primary);
    font-size: 1.05rem;
    line-height: 1.35;
    font-weight: 650;
  }

  .projects .project-overview-card p {
    min-height: 5.6rem;
    margin-bottom: 0.85rem;
    color: var(--text-secondary);
    font-size: 0.93rem;
    line-height: 1.64;
    font-weight: 400;
  }

  .projects .project-overview-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.35rem;
    align-content: flex-start;
    min-height: 5.7rem;
    margin-top: 0.1rem;
    margin-bottom: 0.9rem;
  }

  .projects .project-overview-tag {
    display: inline-flex;
    align-items: center;
    padding: 0.24rem 0.52rem;
    color: var(--text-secondary);
    background: var(--page-bg);
    border: 1px solid var(--border);
    border-radius: 999px;
    font-size: 0.76rem;
    line-height: 1.25;
    font-weight: 500;
  }

  .projects .project-overview-link {
    align-self: flex-start;
    margin-top: auto;
    padding: 0.36rem 0.68rem;
    color: var(--project-accent);
    background: var(--page-bg);
    border: 1px solid var(--project-accent);
    border-radius: 999px;
    font-size: 0.8rem;
    line-height: 1.3;
    font-weight: 600;
  }

  .projects .project-overview-link:hover {
    color: var(--project-accent);
    text-decoration: none;
  }

  html:not([data-theme="dark"]) .projects .project-overview,
  html:not([data-theme="dark"]) .projects .project-overview h2,
  html:not([data-theme="dark"]) .projects .project-overview-intro,
  html:not([data-theme="dark"]) .projects .project-overview-note,
  html:not([data-theme="dark"]) .projects .project-case-studies h2,
  html:not([data-theme="dark"]) .projects .project-case-studies-intro,
  html:not([data-theme="dark"]) .projects .project-overview-card,
  html:not([data-theme="dark"]) .projects .project-overview-card h3,
  html:not([data-theme="dark"]) .projects .project-overview-card p,
  html:not([data-theme="dark"]) .projects .project-overview-tag {
    color: #333333 !important;
  }

  html:not([data-theme="dark"]) .projects .project-overview-card {
    background: #fafafa;
    border-color: #dedede;
    border-top-color: var(--project-accent);
  }

  html:not([data-theme="dark"]) .projects .project-overview-image-wrap {
    background: #f1f1f1;
    border-color: #dedede;
  }

  html:not([data-theme="dark"]) .projects .project-overview-placeholder,
  html:not([data-theme="dark"]) .projects .project-detail-placeholder {
    color: #333333;
    background:
      linear-gradient(135deg, rgba(47, 80, 104, 0.12), rgba(47, 80, 104, 0.035)),
      #f5f7f8;
  }

  html:not([data-theme="dark"]) .projects .project-overview-placeholder span,
  html:not([data-theme="dark"]) .projects .project-detail-placeholder span {
    color: #333333;
  }

  html:not([data-theme="dark"]) .projects .project-overview-label,
  html:not([data-theme="dark"]) .projects .project-overview-link {
    color: var(--project-accent) !important;
  }

  html:not([data-theme="dark"]) .projects .project-overview-tag {
    background: #ffffff;
    border-color: #d8d8d8;
  }

  html:not([data-theme="dark"]) .projects .project-overview-link,
  html:not([data-theme="dark"]) .projects .project-index {
    background: #ffffff;
    border-color: var(--project-accent);
  }

  html:not([data-theme="dark"]) .projects .project-carousel-control {
    background: #ffffff;
    border-color: #2f5068;
  }

  html:not([data-theme="dark"]) .projects .project-carousel-control:disabled {
    border-color: #d8d8d8;
  }

  @media (max-width: 1000px) {
    .projects .project-overview-grid {
      grid-auto-columns: calc((100% - 1rem) / 2);
      gap: 1rem;
    }
  }

  @media (max-width: 680px) {
    .projects .project-carousel-controls {
      display: none;
    }

    .projects .project-overview-grid {
      display: flex;
      gap: 1.25rem;
      overflow-x: auto;
      padding: 0.1rem 0 0.9rem;
      scroll-padding-inline: 0;
      scroll-snap-type: x mandatory;
    }

    .projects .project-overview-card {
      width: min(100%, calc(100vw - 2rem));
      min-width: min(100%, calc(100vw - 2rem));
      height: auto;
      flex: 0 0 min(100%, calc(100vw - 2rem));
      min-height: 0;
      scroll-snap-align: start;
    }

    .projects .project-overview-content {
      grid-template-rows: auto;
      padding: 1rem;
    }

    .projects .project-overview-label,
    .projects .project-overview-card h3,
    .projects .project-overview-card p,
    .projects .project-overview-tags {
      min-height: 0;
    }
  }
</style>

<div class="projects">
  <section class="project-overview" id="selected-projects">
    <h2>Overview</h2>
    <p class="project-overview-intro">
      Applied human factors, healthcare systems, simulation, usability, and performance research across transportation,
      aviation, clinical, and educational settings.
    </p>
    <p class="project-overview-note">Select <strong>View Project</strong> on any card to jump to the full case study below.</p>

    <div class="project-carousel-shell">
      <div class="project-carousel-controls" aria-label="Selected Projects carousel controls">
        <button class="project-carousel-control" type="button" data-carousel-direction="prev" aria-label="Previous selected project">
          <i class="fa-solid fa-arrow-left" aria-hidden="true"></i>
        </button>
        <button class="project-carousel-control" type="button" data-carousel-direction="next" aria-label="Next selected project">
          <i class="fa-solid fa-arrow-right" aria-hidden="true"></i>
        </button>
      </div>

      <div class="project-overview-grid" aria-label="Selected Projects carousel">
        <article class="project-overview-card" id="project-overview-first">
          <div class="project-overview-image-wrap">
            <img
              class="project-overview-image"
              src="{{ '/assets/img/projects/driving/driving-simulator.png' | relative_url }}"
              alt="Driving simulator used for novice teen driver hazard anticipation assessment"
              onerror="this.style.display='none';"
            >
          </div>
          <div class="project-overview-content">
            <span class="project-overview-label"><span class="project-index">01</span> Driving Safety / Human Performance</span>
            <h3>Tablet-Based Hazard Anticipation Training for Novice Teen Drivers</h3>
            <p>
              Studied teen driver training and hazard anticipation using driving simulation, eye tracking, and performance-based
              assessment to evaluate situation awareness and transfer of training.
            </p>
            <div class="project-overview-tags" aria-label="Methods">
              <span class="project-overview-tag">Driving Simulation</span>
              <span class="project-overview-tag">Teen Driver Training</span>
              <span class="project-overview-tag">Eye Tracking</span>
              <span class="project-overview-tag">Situation Awareness</span>
              <span class="project-overview-tag">Training Evaluation</span>
            </div>
            <a class="project-overview-link" href="#driving-safety">View Project</a>
          </div>
        </article>

        <article class="project-overview-card">
          <div class="project-overview-image-wrap">
            <img
              class="project-overview-image"
              src="{{ '/assets/img/projects/aviation/flight-simulator.jpg' | relative_url }}"
              alt="Flight simulator cockpit used for general aviation pilot training research"
              onerror="this.style.display='none';"
            >
          </div>
          <div class="project-overview-content">
            <span class="project-overview-label"><span class="project-index">02</span> Aviation Human Factors</span>
            <h3>Design and Evaluation of Gaze-Based Training for General Aviation Pilots</h3>
            <p>
              Designed and evaluated gaze-based training for VFR-into-IMC transitions using expert gaze, commentary, eye
              tracking, and flight simulation.
            </p>
            <div class="project-overview-tags" aria-label="Methods">
              <span class="project-overview-tag">Aviation HF</span>
              <span class="project-overview-tag">Flight Simulation</span>
              <span class="project-overview-tag">Eye Tracking</span>
              <span class="project-overview-tag">Situation Awareness</span>
              <span class="project-overview-tag">Transfer of Training</span>
            </div>
            <a class="project-overview-link" href="#aviation-human-factors">View Project</a>
          </div>
        </article>

        <article class="project-overview-card">
          <div class="project-overview-image-wrap">
            <img
              class="project-overview-image"
              src="{{ '/assets/img/projects/aviation/pilot-data-synchronization-flow.png' | relative_url }}"
              alt="Pilot data synchronization workflow for multimodal training analysis"
              onerror="this.style.display='none';"
            >
          </div>
          <div class="project-overview-content">
            <span class="project-overview-label"><span class="project-index">03</span> Aviation Analytics / Vocal Stress</span>
            <h3>Multimodal Assessment of Pilot Performance and Vocal Stress</h3>
            <p>
              Integrated gaze, flight-control, aircraft-state, performance, and voice data to evaluate training effects beyond
              visual scanning.
            </p>
            <div class="project-overview-tags" aria-label="Methods">
              <span class="project-overview-tag">Multimodal ML</span>
              <span class="project-overview-tag">SHAP</span>
              <span class="project-overview-tag">CNN</span>
              <span class="project-overview-tag">Voice Analysis</span>
              <span class="project-overview-tag">Data Synchronization</span>
            </div>
            <a class="project-overview-link" href="#pilot-performance-vocal-stress">View Project</a>
          </div>
        </article>

        <article class="project-overview-card">
          <div class="project-overview-image-wrap">
            <img
              class="project-overview-image"
              src="{{ '/assets/img/projects/houston_methodist/nurse-workflow.jpg' | relative_url }}"
              alt="Clinical human factors and hospital workflow setting"
              onerror="this.style.display='none';"
            >
          </div>
          <div class="project-overview-content">
            <span class="project-overview-label"><span class="project-index">04</span> Clinical Human Factors</span>
            <h3>Naturalistic Stress and Workload Monitoring in ICU Nurses</h3>
            <p>
              Applied wearable sensing, eye tracking, and statistical modeling to study ICU nurse stress, workload, and clinical
              work systems.
            </p>
            <div class="project-overview-tags" aria-label="Methods">
              <span class="project-overview-tag">Clinical HF</span>
              <span class="project-overview-tag">Wearables</span>
              <span class="project-overview-tag">Eye Tracking</span>
              <span class="project-overview-tag">Workload</span>
              <span class="project-overview-tag">Mixed-Effects Modeling</span>
            </div>
            <a class="project-overview-link" href="#clinician-stress-workload">View Project</a>
          </div>
        </article>

        <article class="project-overview-card">
          <div class="project-overview-image-wrap">
            <img
              class="project-overview-image"
              src="{{ '/assets/img/projects/mental-health/healthcare-worker-mental-health.jpg' | relative_url }}"
              alt="Healthcare worker wearing a mask and showing signs of stress"
              onerror="this.style.display='none';"
            >
          </div>
          <div class="project-overview-content">
            <span class="project-overview-label"><span class="project-index">05</span> Digital Health / Healthcare Worker Well-Being</span>
            <h3>Digital Positive-Emotion Intervention for Healthcare Worker Mental Health</h3>
            <p>
              Evaluated a Virgin Pulse mobile positive-emotion intervention and modeled changes in mental health, emotion, and
              burnout outcomes.
            </p>
            <div class="project-overview-tags" aria-label="Methods">
              <span class="project-overview-tag">Digital Health</span>
              <span class="project-overview-tag">Mental Health</span>
              <span class="project-overview-tag">Positive Emotion</span>
              <span class="project-overview-tag">Burnout</span>
              <span class="project-overview-tag">Mixed-Effects Modeling</span>
            </div>
            <a class="project-overview-link" href="#healthcare-worker-mental-health">View Project</a>
          </div>
        </article>

        <article class="project-overview-card">
          <div class="project-overview-image-wrap">
            <img
              class="project-overview-image"
              src="{{ '/assets/img/projects/vascular-access/usgva-simulation-procedure.png' | relative_url }}"
              alt="Simulation-based ultrasound-guided vascular access procedure"
              onerror="this.style.display='none';"
            >
          </div>
          <div class="project-overview-content">
            <span class="project-overview-label"><span class="project-index">06</span> Healthcare Systems</span>
            <h3>Hierarchical Task Analysis of Ultrasound-Guided Vascular Access Procedures</h3>
            <p>
              Used task analysis, simulation video, and procedural timing to study ultrasound-guided vascular access workflows
              and microskills.
            </p>
            <div class="project-overview-tags" aria-label="Methods">
              <span class="project-overview-tag">Healthcare Systems</span>
              <span class="project-overview-tag">Task Analysis</span>
              <span class="project-overview-tag">HTA</span>
              <span class="project-overview-tag">Simulation</span>
              <span class="project-overview-tag">Patient Safety</span>
            </div>
            <a class="project-overview-link" href="#vascular-access-workflow">View Project</a>
          </div>
        </article>

        <article class="project-overview-card">
          <div class="project-overview-image-wrap">
            <img
              class="project-overview-image"
              src="{{ '/assets/img/projects/outpatient/outpatient-live-chat-communication.jpg' | relative_url }}"
              alt="Healthcare professional using a headset and laptop for patient communication"
              onerror="this.style.display='none';"
            >
          </div>
          <div class="project-overview-content">
            <span class="project-overview-label"><span class="project-index">07</span> Healthcare Operations</span>
            <h3>Outpatient Appointment Compliance and Live Chat Communication</h3>
            <p>
              Analyzed outpatient appointment data to evaluate live chat/text-based communication and attendance, cancellation,
              rescheduling, and no-show patterns.
            </p>
            <div class="project-overview-tags" aria-label="Methods">
              <span class="project-overview-tag">Healthcare Operations</span>
              <span class="project-overview-tag">Interrupted Time Series</span>
              <span class="project-overview-tag">Patient Access</span>
              <span class="project-overview-tag">Data Analysis</span>
              <span class="project-overview-tag">Process Improvement</span>
            </div>
            <a class="project-overview-link" href="#outpatient-compliance-live-chat">View Project</a>
          </div>
        </article>

        <article class="project-overview-card" id="project-overview-last">
          <div class="project-overview-image-wrap">
            <img
              class="project-overview-image"
              src="{{ '/assets/img/projects/su2c/patient-navigation-app.png' | relative_url }}"
              alt="Digital patient navigation app for breast cancer care"
              onerror="this.style.display='none';"
            >
          </div>
          <div class="project-overview-content">
            <span class="project-overview-label"><span class="project-index">08</span> Digital Health / Usability</span>
            <h3>User-Centered Design of a Digital Patient Navigation Tool for Breast Cancer Care</h3>
            <p>Evaluated usability, patient-facing digital health design, and engagement considerations for mobile health technology.</p>
            <div class="project-overview-tags" aria-label="Methods">
              <span class="project-overview-tag">Digital Health</span>
              <span class="project-overview-tag">UX/UI</span>
              <span class="project-overview-tag">Usability</span>
              <span class="project-overview-tag">Patient Engagement</span>
              <span class="project-overview-tag">Mobile Health</span>
            </div>
            <a class="project-overview-link" href="#digital-health-usability">View Project</a>
          </div>
        </article>
      </div>
    </div>

  </section>

  <script>
    document.addEventListener("DOMContentLoaded", function () {
      document.querySelectorAll(".project-carousel-shell").forEach(function (shell) {
        var scroller = shell.querySelector(".project-overview-grid");
        var previousButton = shell.querySelector('[data-carousel-direction="prev"]');
        var nextButton = shell.querySelector('[data-carousel-direction="next"]');

        if (!scroller || !previousButton || !nextButton) {
          return;
        }

        var getCards = function () {
          return Array.prototype.slice.call(scroller.querySelectorAll(".project-overview-card"));
        };

        var getMaxScrollLeft = function () {
          return Math.max(0, scroller.scrollWidth - scroller.clientWidth);
        };

        var getCardTargetLeft = function (card) {
          var cardRect = card.getBoundingClientRect();
          var scrollerRect = scroller.getBoundingClientRect();
          var targetLeft = cardRect.left - scrollerRect.left + scroller.scrollLeft;

          return Math.min(Math.max(0, targetLeft), getMaxScrollLeft());
        };

        var getCardTargets = function () {
          var targets = getCards().map(getCardTargetLeft);

          return targets.filter(function (target, index) {
            return index === 0 || Math.abs(target - targets[index - 1]) > 2;
          });
        };

        var getCurrentTargetIndex = function (targets) {
          var scrollLeft = Math.max(0, scroller.scrollLeft);
          var closestIndex = 0;
          var closestDistance = Number.POSITIVE_INFINITY;

          targets.forEach(function (target, index) {
            var distance = Math.abs(target - scrollLeft);

            if (distance < closestDistance) {
              closestIndex = index;
              closestDistance = distance;
            }
          });

          return closestIndex;
        };

        var scrollToTarget = function (direction) {
          var targets = getCardTargets();

          if (!targets.length) {
            return;
          }

          var tolerance = 3;
          var scrollLeft = Math.max(0, scroller.scrollLeft);
          var targetIndex;

          if (direction === "prev") {
            targetIndex = -1;

            for (var index = targets.length - 1; index >= 0; index -= 1) {
              if (targets[index] < scrollLeft - tolerance) {
                targetIndex = index;
                break;
              }
            }
          } else {
            targetIndex = targets.findIndex(function (target) {
              return target > scrollLeft + tolerance;
            });
          }

          if (targetIndex === -1) {
            targetIndex = direction === "prev" ? 0 : targets.length - 1;
          }

          scroller.scrollTo({ left: targets[targetIndex], behavior: "smooth" });
        };

        var updateControls = function () {
          var targets = getCardTargets();
          var tolerance = 3;

          if (!targets.length) {
            previousButton.disabled = true;
            nextButton.disabled = true;
            return;
          }

          var currentIndex = getCurrentTargetIndex(targets);
          var scrollLeft = Math.max(0, scroller.scrollLeft);
          var firstTarget = targets[0];
          var lastTarget = targets[targets.length - 1];

          previousButton.disabled = currentIndex === 0 && scrollLeft <= firstTarget + tolerance;
          nextButton.disabled = currentIndex === targets.length - 1 && scrollLeft >= lastTarget - tolerance;
        };

        var requestUpdate = function () {
          window.requestAnimationFrame(updateControls);
        };

        previousButton.addEventListener("click", function () {
          scrollToTarget("prev");
        });

        nextButton.addEventListener("click", function () {
          scrollToTarget("next");
        });

        scroller.addEventListener("scroll", requestUpdate, { passive: true });
        window.addEventListener("resize", requestUpdate);
        updateControls();
      });
    });
  </script>

  <section class="project-case-studies" aria-labelledby="project-case-studies-heading">
    <h2 id="project-case-studies-heading">Projects</h2>
    <p class="project-case-studies-intro">
      Detailed project sections below include methods, results, and supporting visuals for each selected project.
    </p>
  </section>

  <div class="card mt-3" id="driving-safety">
    <div class="card-body project-header">
      <div class="project-category"><span class="project-index">01</span><i class="fa-solid fa-car-side" aria-hidden="true"></i> Driving Safety / Human Performance</div>
      <h5 class="card-title">Tablet-Based Hazard Anticipation Training for Novice Teen Drivers</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/driving/driving-simulator.png' | relative_url }}"
      alt="Driving simulator used for novice teen driver hazard anticipation assessment"
    >
    <div class="card-body">
      <h6 class="project-detail-heading">Overview</h6>
      <p class="card-text">
        This project evaluated the Engaged Driver Training System (EDTS), a tablet-based hazard anticipation training program for
        novice teen drivers. The study examined whether training improved drivers' ability to detect, understand, and anticipate
        latent roadway hazards across simulator and field settings.
      </p>
      <h6 class="project-detail-heading">Study population/setting</h6>
      <ul class="project-detail-list">
        <li>Novice teen driver safety study conducted through ATRANS at Western New England University.</li>
        <li>Combined tablet-based training, driving simulator assessment, and field driving assessment.</li>
      </ul>
      <h6 class="project-detail-heading">Methods and tools</h6>
      <div class="project-method-tags" aria-label="Methods and tools">
        <span class="project-overview-tag">Eye tracking</span>
        <span class="project-overview-tag">Driving simulation</span>
        <span class="project-overview-tag">Field driving assessment</span>
        <span class="project-overview-tag">Commentary driving</span>
        <span class="project-overview-tag">Verbal protocol analysis</span>
        <span class="project-overview-tag">Situation awareness</span>
        <span class="project-overview-tag">Transfer of training</span>
      </div>
      <h6 class="project-detail-heading">Key contributions or findings</h6>
      <ul class="project-detail-list">
        <li>Evaluated a tablet-based hazard anticipation training system for novice teen drivers.</li>
        <li>Assessed roadway scanning, hazard anticipation, and situation awareness.</li>
        <li>Connected simulator assessment with field driving to evaluate transfer of training.</li>
      </ul>
      <div class="row mt-3">
        <div class="col-md-4 mb-3 mb-md-0">
          <img
            class="img-fluid rounded"
            src="{{ '/assets/img/projects/driving/tablet-training-system.png' | relative_url }}"
            alt="Tablet-based EDTS hazard anticipation training system"
          >
          <p class="caption mt-2 mb-0">Tablet-based EDTS training system used to practice identifying latent roadway hazards.</p>
        </div>
        <div class="col-md-4 mb-3 mb-md-0">
          <img
            class="img-fluid rounded"
            src="{{ '/assets/img/projects/driving/field-drive-assessment.png' | relative_url }}"
            alt="Field driving assessment for teen driver hazard perception"
          >
          <p class="caption mt-2 mb-0">Field driving assessment used to evaluate hazard perception and transfer beyond the simulator.</p>
        </div>
        <div class="col-md-4">
          <img
            class="img-fluid rounded"
            src="{{ '/assets/img/projects/driving/on-road-hazard-view.png' | relative_url }}"
            alt="Driver point-of-view roadway hazard scene"
          >
          <p class="caption mt-2 mb-0">Driver point-of-view hazard scene used to assess roadway scanning, hazard anticipation, and situation awareness.</p>
        </div>
      </div>
    </div>
  </div>

  <div class="card mt-3" id="aviation-human-factors">
    <div class="card-body project-header">
      <div class="project-category"><span class="project-index">02</span><i class="fa-solid fa-plane-up" aria-hidden="true"></i> Aviation Training / Human Performance</div>
      <h5 class="card-title">Design and Evaluation of Gaze-Based Training for General Aviation Pilots</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/aviation/flight-simulator.jpg' | relative_url }}"
      alt="Flight simulator cockpit used for general aviation pilot training research"
    >
    <div class="card-body">
      <h6 class="project-detail-heading">Overview</h6>
      <p class="card-text">
        This project designed and evaluated a gaze-based training intervention for general aviation pilots during inadvertent
        transitions from visual flight rules into instrument meteorological conditions. The work used eye tracking, flight
        simulation, expert gaze, and commentary to assess changes in visual scanning, situation awareness, transfer of training,
        and aircraft-control outcomes.
      </p>
      <h6 class="project-detail-heading">Study population/setting</h6>
      <ul class="project-detail-list">
        <li>General aviation student pilot training research conducted in a flight simulator setting.</li>
        <li>Focused on VFR-into-IMC transition scenarios and instrument scanning behavior.</li>
      </ul>
      <h6 class="project-detail-heading">Methods and tools</h6>
      <div class="project-method-tags" aria-label="Methods and tools">
        <span class="project-overview-tag">Eye tracking</span>
        <span class="project-overview-tag">Flight simulation</span>
        <span class="project-overview-tag">Expert gaze</span>
        <span class="project-overview-tag">Expert commentary</span>
        <span class="project-overview-tag">3M training</span>
        <span class="project-overview-tag">Shannon entropy</span>
        <span class="project-overview-tag">Kullback-Leibler divergence</span>
      </div>
      <h6 class="project-detail-heading">Key contributions or findings</h6>
      <ul class="project-detail-list">
        <li>Designed and evaluated a gaze-based aviation training intervention.</li>
        <li>Assessed visual scanning, situation awareness, and transfer of training.</li>
        <li>After training, experimental pilots increased attention to primary instruments.</li>
        <li>After training, experimental pilots reduced visual search randomness and maintained aircraft control during IMC scenarios.</li>
      </ul>
      <div class="row mt-3 justify-content-center">
        <div class="col-md-8">
          <img
            class="img-fluid rounded"
            src="{{ '/assets/img/projects/aviation/eye-tracker.JPG' | relative_url }}"
            alt="Eye-tracking setup used for gaze-based pilot training"
          >
          <p class="caption mt-2 mb-0">Eye-tracking setup used for gaze-based pilot training and data collection.</p>
        </div>
      </div>
      <div class="row mt-3">
        <div class="col-sm-6 mb-3 mb-sm-0">
          <img
            class="img-fluid rounded w-100"
            style="height: 260px; object-fit: cover;"
            src="{{ '/assets/img/projects/aviation/pre-training-gaze-distribution.png' | relative_url }}"
            alt="Pre-training gaze distribution across cockpit instruments"
          >
          <p class="caption mt-2 mb-0"><strong>Before Training:</strong> Pre-training gaze distribution showing dispersed visual attention across cockpit instruments.</p>
        </div>
        <div class="col-sm-6">
          <img
            class="img-fluid rounded w-100"
            style="height: 260px; object-fit: cover;"
            src="{{ '/assets/img/projects/aviation/post-training-gaze-distribution.png' | relative_url }}"
            alt="Post-training gaze distribution focused on primary flight instruments"
          >
          <p class="caption mt-2 mb-0"><strong>After Training:</strong> Post-training gaze distribution showing more focused visual attention on primary flight instruments.</p>
        </div>
      </div>
    </div>
  </div>

  <div class="card mt-3" id="pilot-performance-vocal-stress">
    <div class="card-body project-header">
      <div class="project-category"><span class="project-index">03</span><i class="fa-solid fa-wave-square" aria-hidden="true"></i> Aviation Analytics / Vocal Stress</div>
      <h5 class="card-title">Multimodal Assessment of Pilot Performance and Vocal Stress</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/aviation/pilot-data-synchronization-flow.png' | relative_url }}"
      alt="Pilot data synchronization workflow for multimodal training analysis"
    >
    <div class="card-body">
      <h6 class="project-detail-heading">Overview</h6>
      <p class="card-text">
        This project developed a multimodal framework to evaluate whether aviation training effects extended beyond visual
        scanning behavior. The analysis synchronized gaze, flight-control, aircraft-state, performance, and voice data to assess
        pilot performance and vocal stress during simulated VFR-into-IMC flight.
      </p>
      <h6 class="project-detail-heading">Methods and tools</h6>
      <div class="project-method-tags" aria-label="Methods and tools">
        <span class="project-overview-tag">Data synchronization</span>
        <span class="project-overview-tag">Eye tracking</span>
        <span class="project-overview-tag">Flight-control data</span>
        <span class="project-overview-tag">Aircraft-state data</span>
        <span class="project-overview-tag">Voice data</span>
        <span class="project-overview-tag">Multimodal machine learning</span>
        <span class="project-overview-tag">SHAP</span>
        <span class="project-overview-tag">CNN vocal-stress analysis</span>
      </div>
      <h6 class="project-detail-heading">Key contributions or findings</h6>
      <ul class="project-detail-list">
        <li>Synchronized eye-movement, flight-control, aircraft-state, performance, and voice data.</li>
        <li>Used multimodal machine-learning classification to assess training-related differences.</li>
        <li>Used SHAP-based interpretation to examine model behavior.</li>
        <li>Analyzed voice data separately using a CNN-based vocal stress model.</li>
        <li>Assessed training effects beyond visual scanning behavior.</li>
      </ul>
      <div class="row mt-3 justify-content-center">
        <div class="col-md-10">
          <img
            class="img-fluid rounded w-100"
            src="{{ '/assets/img/projects/aviation/pilot-data-synchronization-flow.png' | relative_url }}"
            alt="Pilot data synchronization workflow for multimodal training analysis"
          >
          <p class="caption mt-2 mb-0">Pilot data synchronization workflow linking eye-movement, voice, flight-control, aircraft-state, and flight performance data.</p>
        </div>
      </div>
      <div class="row mt-3 justify-content-center">
        <div class="col-md-10">
          <img
            class="img-fluid rounded w-100"
            src="{{ '/assets/img/projects/aviation/multimodal-pilot-training-vocal-stress.png' | relative_url }}"
            alt="Multimodal pilot training and vocal stress analysis"
          >
          <p class="caption mt-2 mb-0">Multimodal framework for assessing pilot training effectiveness and vocal stress using synchronized flight, gaze, and voice data.</p>
        </div>
      </div>
    </div>
  </div>

  <div class="card mt-3" id="clinician-stress-workload">
    <div class="card-body project-header">
      <div class="project-category"><span class="project-index">04</span><i class="fa-solid fa-heart-pulse" aria-hidden="true"></i> Healthcare Human Factors / Clinical Workflow</div>
      <h5 class="card-title">Naturalistic Stress and Workload Monitoring in ICU Nurses</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/icu/icu-wearable-sensor-setup.png' | relative_url }}"
      alt="Wearable sensor setup for ICU nurse stress and workload monitoring"
    >
    <div class="card-body">
      <h6 class="project-detail-heading">Overview</h6>
      <p class="card-text">
        This research examined stress, workload, and physiological responses among intensive care unit nurses during real
        clinical shifts. The broader program connected naturalistic workload monitoring with longitudinal work on occupational
        stress and burnout among ICU nurses during the COVID-19 pandemic.
      </p>
      <h6 class="project-detail-heading">Study population/setting</h6>
      <ul class="project-detail-list">
        <li>Physiological data from 23 cardiovascular ICU nurses were analyzed in one study.</li>
        <li>Eye-tracking data from 21 ICU nurses, and complete eye-tracking plus physiological data from 15 nurses, were collected across day and night shifts in a related workload study.</li>
        <li>Longitudinal work included COVID and non-COVID units, repeated 12-hour shifts, validated questionnaires, wearable physiological data, and qualitative shift-level responses.</li>
      </ul>
      <h6 class="project-detail-heading">Methods and tools</h6>
      <div class="project-method-tags" aria-label="Methods and tools">
        <span class="project-overview-tag">Naturalistic clinical study design</span>
        <span class="project-overview-tag">Empatica E4</span>
        <span class="project-overview-tag">Tobii Pro Glasses 2</span>
        <span class="project-overview-tag">Axivity AX3</span>
        <span class="project-overview-tag">Baevsky Stress Index</span>
        <span class="project-overview-tag">Gaze entropy</span>
        <span class="project-overview-tag">Mixed-effects modeling</span>
        <span class="project-overview-tag">Ordinal regression</span>
      </div>
      <h6 class="project-detail-heading">Key contributions or findings</h6>
      <ul class="project-detail-list">
        <li>Analyzed physiological stress signals including heart rate, electrodermal activity, and skin temperature.</li>
        <li>Examined workload and stress through gaze behavior, fixation patterns, pupil diameter, gaze entropy, and Baevsky Stress Index.</li>
        <li>Connected wearable sensing, eye tracking, validated questionnaires, and qualitative shift-level responses in clinical research.</li>
      </ul>
      <div class="row mt-3">
        <div class="col-sm-6 mb-3 mb-sm-0">
          <img
            class="img-fluid rounded"
            src="{{ '/assets/img/projects/icu/empatica-e4-wristband.png' | relative_url }}"
            alt="Empatica E4 wrist sensor for physiological stress monitoring"
          >
          <p class="caption mt-2 mb-0">Empatica E4 wrist sensor used to collect physiological stress signals including heart rate, electrodermal activity, and skin temperature.</p>
        </div>
        <div class="col-sm-6">
          <img
            class="img-fluid rounded"
            src="{{ '/assets/img/projects/icu/houston-methodist-postdoc-office.JPG' | relative_url }}"
            alt="Houston Methodist postdoctoral research workspace"
          >
          <p class="caption mt-2 mb-0">Postdoctoral research workspace at Houston Methodist Center for Outcomes Research.</p>
        </div>
      </div>
    </div>
  </div>

  <div class="card mt-3" id="healthcare-worker-mental-health">
    <div class="card-body project-header">
      <div class="project-category"><span class="project-index">05</span><i class="fa-solid fa-face-smile" aria-hidden="true"></i> Digital Health / Healthcare Worker Well-Being</div>
      <h5 class="card-title">Digital Positive-Emotion Intervention for Healthcare Worker Mental Health</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/mental-health/healthcare-worker-mental-health.jpg' | relative_url }}"
      alt="Healthcare worker wearing a mask and showing signs of stress"
    >
    <div class="card-body">
      <h6 class="project-detail-heading">Overview</h6>
      <p class="card-text">
        This project evaluated a mobile positive-emotion intervention delivered through the Virgin Pulse platform for healthcare
        workers. The analysis examined changes in anxiety, depression, positive emotion, negative emotion, emotional diversity,
        and burnout.
      </p>
      <h6 class="project-detail-heading">Study population/setting</h6>
      <ul class="project-detail-list">
        <li>The primary sample included 137 healthcare workers.</li>
        <li>Fifty participants had measurements at pre-, mid-, and post-intervention.</li>
      </ul>
      <h6 class="project-detail-heading">Methods and tools</h6>
      <div class="project-method-tags" aria-label="Methods and tools">
        <span class="project-overview-tag">Virgin Pulse platform</span>
        <span class="project-overview-tag">Mobile intervention</span>
        <span class="project-overview-tag">Positive emotion</span>
        <span class="project-overview-tag">Negative emotion</span>
        <span class="project-overview-tag">Emotional diversity</span>
        <span class="project-overview-tag">Burnout</span>
        <span class="project-overview-tag">Longitudinal mixed-effects modeling</span>
      </div>
      <h6 class="project-detail-heading">Key contributions or findings</h6>
      <ul class="project-detail-list">
        <li>Anxiety and depression decreased significantly.</li>
        <li>Positive emotion increased and negative emotion decreased significantly.</li>
        <li>Negative emotional diversity decreased.</li>
        <li>Burnout outcomes were not statistically significant.</li>
      </ul>
    </div>
  </div>

  <div class="card mt-3" id="vascular-access-workflow">
    <div class="card-body project-header">
      <div class="project-category"><span class="project-index">06</span><i class="fa-solid fa-diagram-project" aria-hidden="true"></i> Healthcare Human Factors / Clinical Workflow</div>
      <h5 class="card-title">Hierarchical Task Analysis of Ultrasound-Guided Vascular Access Procedures</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/vascular-access/usgva-simulation-procedure.png' | relative_url }}"
      alt="Simulation-based ultrasound-guided vascular access procedure"
    >
    <div class="card-body">
      <h6 class="project-detail-heading">Overview</h6>
      <p class="card-text">
        This project examined ultrasound-guided vascular access procedures performed in a simulation center using first-person
        video, procedural timing, and hierarchical task analysis. The analysis supports future work on procedural efficiency,
        Lean process improvement, targeted microskill training, and ergonomic assessment using RULA.
      </p>
      <h6 class="project-detail-heading">Study population/setting</h6>
      <ul class="project-detail-list">
        <li>Five fellowship-trained emergency medicine physicians performed four procedures on high-fidelity simulators.</li>
        <li>Procedures included peripheral IV placement, single-lumen midline catheter placement, dual-lumen midline catheter placement, and triple-lumen central venous catheter placement.</li>
      </ul>
      <h6 class="project-detail-heading">Methods and tools</h6>
      <div class="project-method-tags" aria-label="Methods and tools">
        <span class="project-overview-tag">Hierarchical task analysis</span>
        <span class="project-overview-tag">Simulation-based assessment</span>
        <span class="project-overview-tag">Tobii Pro Glasses 2</span>
        <span class="project-overview-tag">First-person video analysis</span>
        <span class="project-overview-tag">Procedural timing</span>
        <span class="project-overview-tag">Microskill identification</span>
        <span class="project-overview-tag">RULA assessment</span>
      </div>
      <h6 class="project-detail-heading">Key contributions or findings</h6>
      <ul class="project-detail-list">
        <li>Identified supraordinate tasks, subtasks, and microskills required for each procedure.</li>
        <li>Connected workflow analysis with procedural timing and simulation-based assessment.</li>
        <li>Supported future work on procedural efficiency, Lean process improvement, microskill training, and ergonomics.</li>
      </ul>
    </div>
  </div>

  <div class="card mt-3" id="outpatient-compliance-live-chat">
    <div class="card-body project-header">
      <div class="project-category"><span class="project-index">07</span><i class="fa-solid fa-comments" aria-hidden="true"></i> Healthcare Operations / Patient Access</div>
      <h5 class="card-title">Outpatient Appointment Compliance and Live Chat Communication</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/outpatient/outpatient-live-chat-communication.jpg' | relative_url }}"
      alt="Healthcare professional using a headset and laptop for patient communication"
    >
    <div class="card-body">
      <h6 class="project-detail-heading">Overview</h6>
      <p class="card-text">
        This healthcare systems project evaluated how a multi-modal patient communication system, including live chat and
        text-based reminders, was associated with outpatient appointment attendance, cancellations, rescheduling, and no-show
        patterns in a large healthcare setting.
      </p>
      <h6 class="project-detail-heading">Methods and tools</h6>
      <div class="project-method-tags" aria-label="Methods and tools">
        <span class="project-overview-tag">Healthcare operations</span>
        <span class="project-overview-tag">Outpatient appointment data</span>
        <span class="project-overview-tag">Live chat intervention</span>
        <span class="project-overview-tag">Text reminders</span>
        <span class="project-overview-tag">Patient access</span>
        <span class="project-overview-tag">Interrupted time series</span>
        <span class="project-overview-tag">Quasi-experimental evaluation</span>
      </div>
      <h6 class="project-detail-heading">Key contributions or findings</h6>
      <ul class="project-detail-list">
        <li>Connected patient access, digital communication workflows, and operational analytics.</li>
        <li>Examined attendance, cancellations, rescheduling, and no-show patterns.</li>
        <li>Studied opportunities for improving outpatient appointment compliance.</li>
      </ul>
    </div>
  </div>

  <div class="card mt-3" id="digital-health-usability">
    <div class="card-body project-header">
      <div class="project-category"><span class="project-index">08</span><i class="fa-solid fa-mobile-screen-button" aria-hidden="true"></i> Digital Health UX/UI / Patient Engagement</div>
      <h5 class="card-title">User-Centered Design of a Digital Patient Navigation Tool for Breast Cancer Care</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/su2c/patient-navigation-app.png' | relative_url }}"
      alt="Digital patient navigation app for breast cancer care"
    >
    <div class="card-body">
      <h6 class="project-detail-heading">Overview</h6>
      <p class="card-text">
        This Stand Up To Cancer project focused on the user-centered design and UX/UI evaluation of a culturally tailored,
        app-enhanced patient navigation tool for breast cancer care. The work examined patient needs, hormonal therapy adherence,
        side-effect monitoring, patient-provider communication workflows, and access to support resources.
      </p>
      <h6 class="project-detail-heading">Study population/setting</h6>
      <ul class="project-detail-list">
        <li>Patient-facing digital health work for Black/African American women with ER+ breast cancer.</li>
        <li>Conducted during a postdoctoral fellowship at Houston Methodist Center for Outcomes Research.</li>
      </ul>
      <h6 class="project-detail-heading">Methods and tools</h6>
      <div class="project-method-tags" aria-label="Methods and tools">
        <span class="project-overview-tag">User-centered design</span>
        <span class="project-overview-tag">UX/UI evaluation</span>
        <span class="project-overview-tag">Stakeholder interviews</span>
        <span class="project-overview-tag">Thematic analysis</span>
        <span class="project-overview-tag">MAXQDA</span>
        <span class="project-overview-tag">Functional requirements</span>
        <span class="project-overview-tag">Prototype development</span>
        <span class="project-overview-tag">Usability testing</span>
      </div>
      <h6 class="project-detail-heading">Key contributions or findings</h6>
      <ul class="project-detail-list">
        <li>Evaluated patient-facing digital health design and engagement considerations.</li>
        <li>Supported prototype development and formative usability testing of CareSense pathway and mobile application concepts.</li>
        <li>Connected patient needs assessment, communication workflow analysis, and health equity considerations.</li>
      </ul>
    </div>
  </div>
</div>
