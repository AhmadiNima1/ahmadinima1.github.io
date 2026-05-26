---
layout: page
title: Selected Projects
permalink: /projects/
nav: false
nav_order: 2
---

<div class="projects">
  <div class="card mt-3">
    <img
      class="card-img-top"
      src="{{ '/assets/img/projects/aviation/flight-simulator.jpg' | relative_url }}"
      alt="Flight simulator cockpit used for general aviation pilot training research"
    >
    <div class="card-body">
      <h5 class="card-title">Gaze-Based Training for General Aviation Pilots in VFR-into-IMC Transitions</h5>
      <p class="card-text">
        Developed and evaluated a gaze-based training intervention to improve general aviation student pilots' instrument scanning during inadvertent transition from visual flight rules into instrument meteorological conditions. The study used eye tracking, flight simulation, expert commentary, and 3M training to assess changes in visual attention, situation awareness, and piloting performance. After training, experimental pilots increased attention to primary instruments, reduced visual search randomness, and maintained aircraft control during IMC scenarios.
      </p>
      <p class="card-text">
        <strong>Methods and skills:</strong> Eye tracking, flight simulation, simulation-based training, situation awareness, visual attention, Shannon entropy, Kullback-Leibler divergence, Python-based data synchronization, experimental design, statistical analysis.
      </p>
      <div class="row mt-3">
        <div class="col-sm-6 mb-3 mb-sm-0">
          <img
            class="img-fluid rounded"
            src="{{ '/assets/img/projects/aviation/eye-tracker.JPG' | relative_url }}"
            alt="Eye-tracking setup used for gaze-based pilot training"
          >
          <p class="caption mt-2 mb-0">Eye-tracking setup used for gaze-based pilot training and data collection.</p>
        </div>
        <div class="col-sm-6 mb-3 mb-sm-0">
          <img
            class="img-fluid rounded"
            src="{{ '/assets/img/projects/aviation/pre-training-gaze-distribution.png' | relative_url }}"
            alt="Pre-training gaze distribution across cockpit instruments"
          >
          <p class="caption mt-2 mb-0">Pre-training gaze distribution showing dispersed visual attention across cockpit instruments.</p>
        </div>
        <div class="col-sm-6">
          <img
            class="img-fluid rounded"
            src="{{ '/assets/img/projects/aviation/post-training-gaze-distribution.png' | relative_url }}"
            alt="Post-training gaze distribution focused on primary flight instruments"
          >
          <p class="caption mt-2 mb-0">Post-training gaze distribution showing more focused visual attention on primary flight instruments.</p>
        </div>
      </div>
    </div>
  </div>
</div>
