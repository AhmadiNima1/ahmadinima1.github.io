---
layout: page
title: Selected Projects
permalink: /projects/
nav: false
nav_order: 2
---

<style>
  .projects .card .card-body .card-text {
    color: #e0e0e0 !important;
  }

  .projects .card .card-body .card-text strong,
  .projects .card .card-title {
    color: #ffffff !important;
  }

  .projects .card .caption {
    color: #d8dee9 !important;
  }
</style>

<div class="projects">
  <div class="card mt-3">
    <div class="card-body pb-0">
      <h5 class="card-title">Tablet-Based Hazard Anticipation Training for Novice Teen Drivers</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/driving/driving-simulator.png' | relative_url }}"
      alt="Driving simulator used for novice teen driver hazard anticipation assessment"
    >
    <div class="card-body">
      <p class="card-text">
        As a Graduate Research Assistant in the Center for Advanced Training Research and Naturalistic Studies (ATRANS) at Western New England University, I contributed to a teen driver safety study under the supervision of Dr. Matthew Romoser, in collaboration with Atefeh Katrahmani. The project evaluated the Engaged Driver Training System (EDTS), a tablet-based hazard anticipation training program designed to improve novice teen drivers' ability to detect, understand, and anticipate latent roadway hazards. The study combined tablet-based training, driving simulator assessment, field driving, Tobii eye tracking, and commentary driving/verbal protocol analysis to evaluate situation awareness and transfer of training.
      </p>
      <p class="card-text">
        <strong>Methods and skills:</strong> Eye tracking, driving simulation, field driving assessment, commentary driving, verbal protocol analysis, situation awareness, hazard anticipation, tablet-based training, teen driver safety, human performance assessment, transfer of training.
      </p>
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

  <div class="card mt-3">
    <div class="card-body pb-0">
      <h5 class="card-title">Gaze-Based Training for General Aviation Pilots in VFR-into-IMC Transitions</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/aviation/flight-simulator.jpg' | relative_url }}"
      alt="Flight simulator cockpit used for general aviation pilot training research"
    >
    <div class="card-body">
      <p class="card-text">
        Developed and evaluated a gaze-based training intervention to improve general aviation student pilots' instrument scanning during inadvertent transition from visual flight rules into instrument meteorological conditions. The study used eye tracking, flight simulation, expert commentary, and 3M training to assess changes in visual attention, situation awareness, and piloting performance. This work was also conducted as part of human performance and training research at the Center for Advanced Training Research and Naturalistic Studies (ATRANS). After training, experimental pilots increased attention to primary instruments, reduced visual search randomness, and maintained aircraft control during IMC scenarios.
      </p>
      <p class="card-text">
        <strong>Methods and skills:</strong> Eye tracking, flight simulation, simulation-based training, situation awareness, visual attention, Shannon entropy, Kullback-Leibler divergence, Python-based data synchronization, experimental design, statistical analysis.
      </p>
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
      <h6 class="mt-3">Follow-up Multimodal ML and Vocal Stress Analysis</h6>
      <p class="card-text">
        A follow-up analysis extended this work by using synchronized eye-tracking, flight-control, aircraft-state, and voice data to classify trained versus untrained pilots and assess vocal stress duration. The analysis used Tobii Pro Glasses 2, X-Plane 11 flight simulator data, multimodal machine learning classifiers, and a CNN-based vocal stress model.
      </p>
      <div class="row mt-3">
        <div class="col-sm-6 mb-3 mb-sm-0">
          <img
            class="img-fluid rounded w-100"
            style="height: 260px; object-fit: cover;"
            src="{{ '/assets/img/projects/aviation/pilot-data-synchronization-flow.png' | relative_url }}"
            alt="Pilot data synchronization workflow for multimodal training analysis"
          >
          <p class="caption mt-2 mb-0">Pilot data synchronization workflow linking eye-tracking, flight-control, aircraft-state, and voice data.</p>
        </div>
        <div class="col-sm-6">
          <img
            class="img-fluid rounded w-100"
            style="height: 260px; object-fit: cover;"
            src="{{ '/assets/img/projects/aviation/multimodal-pilot-training-vocal-stress.png' | relative_url }}"
            alt="Multimodal pilot training and vocal stress analysis"
          >
          <p class="caption mt-2 mb-0">Multimodal pilot training and vocal stress analysis using synchronized flight, gaze, and voice data.</p>
        </div>
      </div>
    </div>
  </div>

  <div class="card mt-3">
    <div class="card-body pb-0">
      <h5 class="card-title">Naturalistic Stress and Workload Monitoring in ICU Nurses</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/icu/icu-wearable-sensor-setup.png' | relative_url }}"
      alt="Wearable sensor setup for ICU nurse stress and workload monitoring"
    >
    <div class="card-body">
      <p class="card-text">
        At Houston Methodist, I worked on a series of naturalistic human factors studies examining stress, workload, and physiological responses among intensive care unit nurses during real 12-hour clinical shifts. In one study, physiological data from 23 cardiovascular ICU nurses were analyzed using Empatica E4 signals, including heart rate, electrodermal activity, and skin temperature, to examine physiological correlates of occupational stress. In a related workload study, eye-tracking data from 21 ICU nurses, and complete eye-tracking plus physiological data from 15 nurses, were collected across day and night shifts using Tobii Pro Glasses 2 and Empatica E4. These analyses examined workload and stress through gaze behavior, fixation patterns, pupil diameter, gaze entropy, and Baevsky Stress Index. This broader research program also connected to longitudinal work on occupational stress and burnout among ICU nurses during the COVID-19 pandemic, including COVID and non-COVID units, repeated 12-hour shifts, validated questionnaires, wearable physiological data, and qualitative shift-level responses.
      </p>
      <p class="card-text">
        <strong>Methods and skills:</strong> Naturalistic clinical study design, ICU workflow observation, day/night 12-hour shift data collection, wearable sensing, Empatica E4, Tobii Pro Glasses 2, Axivity AX3, physiological stress monitoring, electrodermal activity, heart rate, skin temperature, Baevsky Stress Index, eye tracking, fixation analysis, pupil response, gaze entropy, workload assessment, COVID/non-COVID ICU stress comparison, mixed-effects modeling, ordinal regression, qualitative analysis, IRB-approved clinical research.
      </p>
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

  <div class="card mt-3">
    <div class="card-body pb-0">
      <h5 class="card-title">User-Centered Design of a Digital Patient Navigation Tool for Breast Cancer Care</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/su2c/patient-navigation-app.png' | relative_url }}"
      alt="Digital patient navigation app for breast cancer care"
    >
    <div class="card-body">
      <p class="card-text">
        During my postdoctoral fellowship at Houston Methodist Center for Outcomes Research, I contributed to a Stand Up To Cancer project focused on the user-centered design of a culturally tailored, app-enhanced patient navigation tool for breast cancer care. The project aimed to support Black/African American women with ER+ breast cancer by improving education, hormonal therapy adherence, side-effect monitoring, patient-provider communication, and access to support resources. The work included semi-structured stakeholder interviews, qualitative thematic analysis, functional information requirement analysis, prototype development, and formative usability testing of a refined CareSense pathway and mobile application concepts.
      </p>
      <p class="card-text">
        <strong>Methods and skills:</strong> User-centered design, healthcare UX research, digital health, patient navigation, breast cancer care, stakeholder interviews, semi-structured interviews, qualitative coding, thematic analysis, MAXQDA, functional information requirement analysis, prototype development, usability testing, CareSense pathway design, patient-centered communication, health equity.
      </p>
    </div>
  </div>

  <div class="card mt-3">
    <div class="card-body pb-0">
      <h5 class="card-title">Hierarchical Task Analysis of Ultrasound-Guided Vascular Access Procedures</h5>
    </div>
    <img
      class="card-img-top"
      style="height: 320px; object-fit: cover; object-position: center;"
      src="{{ '/assets/img/projects/vascular-access/usgva-simulation-procedure.png' | relative_url }}"
      alt="Simulation-based ultrasound-guided vascular access procedure"
    >
    <div class="card-body">
      <p class="card-text">
        This project examines ultrasound-guided vascular access procedures performed in a simulation center using first-person video, procedural timing, and hierarchical task analysis. Five fellowship-trained emergency medicine physicians performed four procedures on high-fidelity simulators: peripheral IV placement, single-lumen midline catheter placement, dual-lumen midline catheter placement, and triple-lumen central venous catheter placement. Tobii Pro Glasses 2 recordings were used to identify supraordinate tasks, subtasks, and microskills required for each procedure. The analysis supports future work on procedural efficiency, Lean process improvement, targeted microskill training, and ergonomic assessment using RULA.
      </p>
      <p class="card-text">
        <strong>Methods and skills:</strong> Hierarchical task analysis, healthcare human factors, simulation-based assessment, ultrasound-guided vascular access, emergency medicine procedures, Tobii Pro Glasses 2, first-person video analysis, procedural timing analysis, microskill identification, Lean process improvement, RULA assessment, workflow analysis, clinical training design.
      </p>
      <p class="card-text">
        <strong>Procedures/devices:</strong> Peripheral IV placement; single-lumen midline catheter placement; dual-lumen midline catheter placement; triple-lumen central venous catheter placement.
      </p>
    </div>
  </div>
</div>
