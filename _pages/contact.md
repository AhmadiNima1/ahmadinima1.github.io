---
layout: page
permalink: /contact/
title: Contact
description:
nav: true
nav_order: 6
---

<style>
  .contact-page {
    color: var(--text-secondary);
  }

  .contact-page .contact-intro {
    max-width: 820px;
    margin-bottom: 1.6rem;
    padding: 0.9rem 1rem;
    color: var(--text-secondary);
    background: var(--card-bg);
    border: 1px solid var(--border);
    border-left: 3px solid var(--accent);
    border-radius: 8px;
    font-size: 0.98rem;
    line-height: 1.65;
  }

  .contact-page .contact-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1.1rem;
    align-items: stretch;
  }

  .contact-page .contact-card {
    position: relative;
    display: flex;
    flex-direction: column;
    gap: 1rem;
    height: 100%;
    min-height: 16.75rem;
    overflow: hidden;
    padding: 1.4rem;
    --contact-card-bg: var(--card-bg);
    --contact-card-wash: var(--accent-soft);
    color: var(--text-secondary);
    background:
      linear-gradient(180deg, var(--contact-card-wash) 0, transparent 5rem),
      var(--contact-card-bg);
    border: 1px solid var(--border);
    border-radius: 8px;
    box-shadow: 0 0.2rem 0.9rem rgba(0, 0, 0, 0.04);
    transition:
      transform 160ms ease,
      border-color 160ms ease,
      box-shadow 160ms ease;
  }

  .contact-page .contact-card:nth-child(1) {
    --contact-card-wash: rgba(83, 116, 145, 0.16);
  }

  .contact-page .contact-card:nth-child(2) {
    --contact-card-wash: rgba(63, 128, 112, 0.16);
  }

  .contact-page .contact-card:nth-child(3) {
    --contact-card-wash: rgba(51, 111, 168, 0.16);
  }

  .contact-page .contact-card::before {
    position: absolute;
    top: 0;
    right: 0;
    left: 0;
    height: 3px;
    background: var(--accent);
    content: "";
  }

  .contact-page .contact-card:hover {
    transform: translateY(-2px);
    border-color: var(--accent);
    box-shadow: 0 0.45rem 1.25rem rgba(0, 0, 0, 0.08);
  }

  .contact-page .contact-card-header {
    display: flex;
    gap: 0.75rem;
    align-items: center;
    padding-bottom: 0.9rem;
    border-bottom: 1px solid var(--border);
  }

  .contact-page .contact-icon {
    flex: 0 0 auto;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 2.45rem;
    height: 2.45rem;
    color: var(--accent);
    background: var(--page-bg);
    border: 1px solid var(--border);
    border-radius: 999px;
    font-size: 1rem;
  }

  .contact-page .contact-card h2 {
    margin: 0;
    color: var(--text-primary);
    font-size: 1.1rem;
    line-height: 1.35;
    font-weight: 600;
  }

  .contact-page .contact-detail {
    display: grid;
    gap: 0.35rem;
    padding: 0.75rem 0.85rem;
    background: var(--page-bg);
    border: 1px solid var(--border);
    border-radius: 8px;
  }

  .contact-page .contact-detail-label {
    color: var(--text-muted);
    font-size: 0.76rem;
    line-height: 1.25;
    font-weight: 700;
    letter-spacing: 0.04em;
    text-transform: uppercase;
  }

  .contact-page .contact-content-link {
    display: inline-flex;
    align-self: flex-start;
    margin: 0;
    color: var(--accent);
    font-size: 0.95rem;
    font-weight: 600;
    overflow-wrap: anywhere;
  }

  .contact-page .email-link {
    white-space: nowrap;
    overflow-wrap: normal !important;
    word-break: normal;
  }

  .contact-page .contact-card p {
    margin: 0;
    color: var(--text-secondary);
    font-size: 0.95rem;
    line-height: 1.6;
  }

  .contact-page .contact-button {
    display: inline-flex;
    align-items: center;
    align-self: flex-start;
    margin-top: auto;
    padding: 0.42rem 0.78rem;
    color: var(--accent);
    background: var(--page-bg);
    border: 1px solid var(--border);
    border-radius: 999px;
    font-size: 0.82rem;
    line-height: 1.25;
    font-weight: 600;
  }

  .contact-page .contact-button:hover {
    color: var(--page-bg);
    background: var(--accent);
    border-color: var(--accent);
    text-decoration: none;
  }

  .contact-page .contact-closing {
    margin: 1.25rem 0 0;
    color: var(--text-muted);
    font-size: 0.95rem;
    line-height: 1.6;
  }

  html:not([data-theme="dark"]) .contact-page,
  html:not([data-theme="dark"]) .contact-page .contact-intro,
  html:not([data-theme="dark"]) .contact-page .contact-card,
  html:not([data-theme="dark"]) .contact-page .contact-card h2,
  html:not([data-theme="dark"]) .contact-page .contact-card p {
    color: #333333;
  }

  html:not([data-theme="dark"]) .contact-page .contact-card {
    --contact-card-bg: #fafafa;
    border-color: #dedede;
  }

  html:not([data-theme="dark"]) .contact-page .contact-card:nth-child(1) {
    --contact-card-bg: #f5f7fa;
    --contact-card-wash: rgba(83, 116, 145, 0.1);
  }

  html:not([data-theme="dark"]) .contact-page .contact-card:nth-child(2) {
    --contact-card-bg: #f4f8f6;
    --contact-card-wash: rgba(63, 128, 112, 0.1);
  }

  html:not([data-theme="dark"]) .contact-page .contact-card:nth-child(3) {
    --contact-card-bg: #f4f8fc;
    --contact-card-wash: rgba(51, 111, 168, 0.1);
  }

  html:not([data-theme="dark"]) .contact-page .contact-card:hover {
    box-shadow: 0 0.45rem 1.25rem rgba(0, 0, 0, 0.08);
  }

  html:not([data-theme="dark"]) .contact-page .contact-intro,
  html:not([data-theme="dark"]) .contact-page .contact-detail {
    background: #ffffff;
    border-color: #dedede;
  }

  html:not([data-theme="dark"]) .contact-page .contact-intro {
    border-left-color: #2f5068;
  }

  html:not([data-theme="dark"]) .contact-page .contact-icon {
    color: #2f5068;
    background: #ffffff;
    border-color: #d8d8d8;
  }

  html:not([data-theme="dark"]) .contact-page .contact-content-link,
  html:not([data-theme="dark"]) .contact-page .contact-button {
    color: #2f5068;
  }

  html:not([data-theme="dark"]) .contact-page .contact-button {
    background: #ffffff;
    border-color: #d8d8d8;
  }

  html:not([data-theme="dark"]) .contact-page .contact-button:hover {
    color: #ffffff;
    background: #2f5068;
    border-color: #2f5068;
  }

  html:not([data-theme="dark"]) .contact-page .contact-closing {
    color: #4a4a4a;
  }

  @media (max-width: 900px) {
    .contact-page .contact-grid {
      grid-template-columns: 1fr;
    }

    .contact-page .contact-card {
      min-height: 0;
    }
  }
</style>

<div class="contact-page">
  <p class="contact-intro">
    I'm happy to connect about human factors, healthcare systems, aviation safety, usability research, simulation, applied AI,
    collaborations, and professional opportunities.
  </p>

  <div class="contact-grid">
    <article class="contact-card">
      <div class="contact-card-header">
        <span class="contact-icon" aria-hidden="true"><i class="fa-solid fa-graduation-cap"></i></span>
        <h2>Academic / RPI</h2>
      </div>
      <div class="contact-detail">
        <span class="contact-detail-label">Email</span>
        <a class="contact-content-link email-link" href="mailto:ahmadn4@rpi.edu">ahmadn4@rpi.edu</a>
      </div>
      <p>For teaching, students, academic collaborations, and university-related communication.</p>
    </article>

    <article class="contact-card">
      <div class="contact-card-header">
        <span class="contact-icon" aria-hidden="true"><i class="fa-solid fa-briefcase"></i></span>
        <h2>Professional / Industry</h2>
      </div>
      <div class="contact-detail">
        <span class="contact-detail-label">Email</span>
        <a class="contact-content-link email-link" href="mailto:ahmadi.nima@gmail.com">ahmadi.nima@gmail.com</a>
      </div>
      <p>
        For industry roles, consulting, human factors opportunities, healthcare systems, usability research, aviation safety,
        and applied AI.
      </p>
    </article>

    <article class="contact-card">
      <div class="contact-card-header">
        <span class="contact-icon" aria-hidden="true"><i class="fa-brands fa-linkedin-in"></i></span>
        <h2>LinkedIn</h2>
      </div>
      <p>Best for networking, referrals, job opportunities, and quick introductions.</p>
      <a class="contact-button" href="https://www.linkedin.com/in/nimahmadi" target="_blank" rel="noopener noreferrer" aria-label="Connect on LinkedIn">
        Connect on LinkedIn
      </a>
    </article>

  </div>

  <p class="contact-closing">Based in the Capital Region, NY. Open to selected remote, hybrid, and relocation opportunities.</p>
</div>
