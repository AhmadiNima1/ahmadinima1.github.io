---
layout: page
permalink: /teaching/
title: Teaching Portfolio
description: Courses taught across human factors, engineering design, simulation, analytics, and computing.
nav: true
nav_order: 4
---

<style>
  .teaching-portfolio {
    --teaching-surface: var(--global-card-bg-color);
    --teaching-border: var(--global-divider-color);
    --teaching-soft: rgba(127, 127, 127, 0.08);
    --teaching-radius: 8px;
    color: var(--global-text-color);
  }

  .teaching-portfolio h2 {
    margin-bottom: 1rem;
    color: var(--global-text-color);
    font-size: 1.52rem;
    line-height: 1.24;
    font-weight: 650;
  }

  .teaching-group {
    margin-bottom: 1.6rem;
  }

  .teaching-group:last-child {
    margin-bottom: 0;
  }

  .teaching-group-title {
    margin: 0 0 0.65rem;
    color: var(--global-text-color);
    font-size: 1.05rem;
    line-height: 1.35;
    font-weight: 650;
  }

  .teaching-table {
    overflow: hidden;
    background: var(--teaching-surface);
    border: 1px solid var(--teaching-border);
    border-radius: var(--teaching-radius);
  }

  .teaching-row {
    display: grid;
    grid-template-columns: minmax(0, 1fr) minmax(14rem, 0.42fr);
    gap: 1.2rem;
    align-items: center;
    padding: 0.95rem 1.1rem;
    border-bottom: 1px solid var(--teaching-border);
  }

  .teaching-row:last-child {
    border-bottom: 0;
  }

  .teaching-header {
    color: var(--global-text-color);
    background: var(--teaching-soft);
    font-size: 0.78rem;
    line-height: 1.25;
    font-weight: 700;
    letter-spacing: 0.02em;
    text-transform: uppercase;
  }

  .teaching-course {
    color: var(--global-text-color);
    font-size: 0.96rem;
    line-height: 1.45;
    font-weight: 550;
  }

  .teaching-area {
    color: var(--global-text-color-light);
    font-size: 0.86rem;
    line-height: 1.45;
    font-weight: 500;
  }

  html[data-theme="dark"] .teaching-portfolio {
    --teaching-soft: rgba(143, 206, 225, 0.08);
  }

  @media (max-width: 575px) {
    .teaching-row {
      grid-template-columns: 1fr;
      gap: 0.35rem;
      padding: 0.95rem 1rem;
    }

    .teaching-header {
      display: none;
    }
  }
</style>

<div class="teaching-portfolio">
  <h2>Courses</h2>

  <div class="teaching-group">
    <h3 class="teaching-group-title">Rensselaer Polytechnic Institute (RPI)</h3>
    <div class="teaching-table" aria-label="Rensselaer Polytechnic Institute courses taught">
      <div class="teaching-row teaching-header">
        <span>Course</span>
        <span>Area</span>
      </div>
      <div class="teaching-row">
        <span class="teaching-course">ISYE 4210/6600 &ndash; Design and Analysis of Supply Chains</span>
        <span class="teaching-area">Systems Engineering</span>
      </div>
      <div class="teaching-row">
        <span class="teaching-course">ISYE 4260/6260 &ndash; Human Performance Modeling and Support</span>
        <span class="teaching-area">Human Factors</span>
      </div>
      <div class="teaching-row">
        <span class="teaching-course">ISYE 4270 &ndash; Multidisciplinary Capstone Design</span>
        <span class="teaching-area">Engineering Design / Capstone</span>
      </div>
      <div class="teaching-row">
        <span class="teaching-course">ISYE 4290/6620 &ndash; Discrete-Event Simulation Modeling and Analysis</span>
        <span class="teaching-area">Healthcare &amp; Manufacturing Simulation</span>
      </div>
      <div class="teaching-row">
        <span class="teaching-course">ISYE 4330/6020 &ndash; Design of Experiments</span>
        <span class="teaching-area">Experimental Design</span>
      </div>
      <div class="teaching-row">
        <span class="teaching-course">ENGR 2600 &ndash; Modeling and Analysis of Uncertainty</span>
        <span class="teaching-area">Statistics / Analytics</span>
      </div>
    </div>
  </div>

  <div class="teaching-group">
    <h3 class="teaching-group-title">Western New England University (WNEU)</h3>
    <div class="teaching-table" aria-label="Western New England University courses taught">
      <div class="teaching-row teaching-header">
        <span>Course</span>
        <span>Area</span>
      </div>
      <div class="teaching-row">
        <span class="teaching-course">IE 212 &ndash; Probability &amp; Statistics</span>
        <span class="teaching-area">Probability &amp; Statistics</span>
      </div>
      <div class="teaching-row">
        <span class="teaching-course">IE 419 &ndash; Industrial Engineering Computer Applications</span>
        <span class="teaching-area">Computing / Industrial Engineering</span>
      </div>
      <div class="teaching-row">
        <span class="teaching-course">ME 205 &ndash; Measurement Computing</span>
        <span class="teaching-area">Measurement / Computing</span>
      </div>
    </div>
  </div>
</div>
