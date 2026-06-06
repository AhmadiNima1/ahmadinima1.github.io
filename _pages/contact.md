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
    margin-bottom: 1.3rem;
    color: var(--text-secondary);
    font-size: 0.98rem;
    line-height: 1.65;
  }

  .contact-page .contact-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    align-items: stretch;
  }

  .contact-page .contact-card {
    display: flex;
    flex-direction: column;
    gap: 0.85rem;
    height: 100%;
    min-height: 15.5rem;
    padding: 1.15rem;
    color: var(--text-secondary);
    background: var(--card-bg);
    border: 1px solid var(--border);
    border-top: 3px solid var(--accent);
    border-radius: 8px;
    transition:
      transform 160ms ease,
      border-color 160ms ease,
      box-shadow 160ms ease;
  }

  .contact-page .contact-card:hover {
    transform: translateY(-2px);
    border-color: var(--accent);
    box-shadow: 0 0.45rem 1.25rem rgba(0, 0, 0, 0.08);
  }

  .contact-page .contact-icon {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 2.2rem;
    height: 2.2rem;
    color: var(--accent);
    background: var(--page-bg);
    border: 1px solid var(--border);
    border-radius: 999px;
    font-size: 0.95rem;
  }

  .contact-page .contact-card h2 {
    margin: 0;
    color: var(--text-primary);
    font-size: 1.1rem;
    line-height: 1.35;
    font-weight: 600;
  }

  .contact-page .contact-content-link {
    display: inline-flex;
    align-self: flex-start;
    margin: 0.1rem 0 0.2rem;
    color: var(--accent);
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
    padding: 0.36rem 0.68rem;
    color: var(--accent);
    background: var(--page-bg);
    border: 1px solid var(--border);
    border-radius: 999px;
    font-size: 0.82rem;
    line-height: 1.25;
    font-weight: 600;
  }

  .contact-page .contact-button:hover {
    color: var(--accent);
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
    background: #fafafa;
    border-color: #dedede;
    border-top-color: #2f5068;
  }

  html:not([data-theme="dark"]) .contact-page .contact-card:hover {
    box-shadow: 0 0.45rem 1.25rem rgba(0, 0, 0, 0.08);
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

  html:not([data-theme="dark"]) .contact-page .contact-closing {
    color: #4a4a4a;
  }

  @media (max-width: 900px) {
    .contact-page .contact-grid {
      grid-template-columns: 1fr;
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
      <span class="contact-icon" aria-hidden="true"><i class="fa-solid fa-graduation-cap"></i></span>
      <h2>Academic / RPI</h2>
      <a class="contact-content-link email-link" href="mailto:ahmadn4@rpi.edu">ahmadn4@rpi.edu</a>
      <p>For teaching, students, academic collaborations, and university-related communication.</p>
    </article>

    <article class="contact-card">
      <span class="contact-icon" aria-hidden="true"><i class="fa-solid fa-briefcase"></i></span>
      <h2>Professional / Industry</h2>
      <a class="contact-content-link email-link" href="mailto:ahmadi.nima@gmail.com">ahmadi.nima@gmail.com</a>
      <p>
        For industry roles, consulting, human factors opportunities, healthcare systems, usability research, aviation safety,
        and applied AI.
      </p>
    </article>

    <article class="contact-card">
      <span class="contact-icon" aria-hidden="true"><i class="fa-brands fa-linkedin-in"></i></span>
      <h2>LinkedIn</h2>
      <p>Connect with me on LinkedIn.</p>
      <p>Best for networking, referrals, job opportunities, and quick introductions.</p>
      <a class="contact-button" href="https://www.linkedin.com/in/nimahmadi" target="_blank" rel="noopener noreferrer" aria-label="Connect on LinkedIn">
        Connect on LinkedIn
      </a>
    </article>

  </div>

  <p class="contact-closing">Based in the Capital Region, NY. Open to selected remote, hybrid, and relocation opportunities.</p>
</div>
