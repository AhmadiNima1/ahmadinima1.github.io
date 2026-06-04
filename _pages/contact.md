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
    color: var(--global-text-color);
  }

  .contact-page .contact-intro {
    max-width: 760px;
    margin-bottom: 1.4rem;
    color: var(--global-text-color);
    font-size: 1rem;
    line-height: 1.7;
  }

  .contact-page .contact-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 1rem;
  }

  .contact-page .contact-card {
    display: flex;
    gap: 0.85rem;
    padding: 1rem;
    color: var(--global-text-color);
    background: var(--global-card-bg-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
  }

  .contact-page .contact-icon {
    flex: 0 0 auto;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 2rem;
    height: 2rem;
    color: var(--global-theme-color);
    background: var(--global-bg-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    font-size: 0.9rem;
  }

  .contact-page .contact-card h2 {
    margin: 0 0 0.25rem;
    color: var(--global-text-color);
    font-size: 1rem;
    font-weight: 700;
  }

  .contact-page .contact-card a {
    display: inline-block;
    margin-bottom: 0.45rem;
    font-weight: 600;
  }

  .contact-page .contact-card p {
    margin: 0;
    color: var(--global-text-color);
    font-size: 0.92rem;
    line-height: 1.55;
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
  }

  html:not([data-theme="dark"]) .contact-page .contact-icon {
    background: #ffffff;
    border-color: #d8d8d8;
  }
</style>

<div class="contact-page">
  <p class="contact-intro">
    I’m always happy to connect about human factors, healthcare systems, aviation safety, simulation, wearable sensing, applied AI, or research collaboration.
  </p>

  <p class="contact-intro">You can reach me in three ways:</p>

  <div class="contact-grid">
    <article class="contact-card">
      <span class="contact-icon" aria-hidden="true"><i class="fa-solid fa-building-columns"></i></span>
      <div>
        <h2>RPI Email</h2>
        <a href="mailto:ahmadn4@rpi.edu">ahmadn4@rpi.edu</a>
        <p>Best for academic, student, or university-related communication.</p>
      </div>
    </article>

    <article class="contact-card">
      <span class="contact-icon" aria-hidden="true"><i class="fa-solid fa-envelope"></i></span>
      <div>
        <h2>Gmail</h2>
        <a href="mailto:ahmadi.nima@gmail.com">ahmadi.nima@gmail.com</a>
        <p>Best for professional, industry, or general inquiries.</p>
      </div>
    </article>

    <article class="contact-card">
      <span class="contact-icon" aria-hidden="true"><i class="fa-brands fa-linkedin-in"></i></span>
      <div>
        <h2>LinkedIn</h2>
        <a href="https://www.linkedin.com/in/nimahmadi" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn profile">Reach out or connect with me on LinkedIn.</a>
        <p>Best for networking, job opportunities, and professional conversations.</p>
      </div>
    </article>

  </div>
</div>
