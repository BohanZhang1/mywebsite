---
permalink: /
title: "Bohan Zhang"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

PhD Candidate in Computer Science at [Saint Louis University](https://www.slu.edu), fully sponsored by the [NASA University Leadership Initiative (ULI)](https://www.nasa.gov/directorates/armd/tacp/ui/uli/). I build simulation and automated testing infrastructure to close the *sim-to-reality gap* for small Uncrewed Aerial Systems (sUAS).

<div style="display:flex; gap:0.6em; flex-wrap:wrap; margin:1.2em 0 1.8em;">
  <span style="background:#003DA5; color:#fff; padding:4px 13px; border-radius:12px; font-size:0.82em; font-weight:500;">NASA ULI Sponsored</span>
  <span style="background:#003DA5; color:#fff; padding:4px 13px; border-radius:12px; font-size:0.82em; font-weight:500;">8 Publications</span>
  <span style="background:#003DA5; color:#fff; padding:4px 13px; border-radius:12px; font-size:0.82em; font-weight:500;">PhD Candidate · SLU 2027</span>
  <span style="background:#003DA5; color:#fff; padding:4px 13px; border-radius:12px; font-size:0.82em; font-weight:500;">IEEE RE · ASE · ICSE · PLANS</span>
</div>

---

## Research

I develop tools that make sUAS simulation testing rigorous, automated, and closer to physical reality.

<div class="site-research-blue" style="background:#eef3fb; padding:12px 16px; margin:5px 0; border-left:4px solid #003DA5; border-radius:0 6px 6px 0; color:#111827;">
<strong><a href="https://github.com/UAVLab-SLU/DRV_public">DroneReqValidator (DRV) / DroneWorld</a></strong><br>
Automated sUAS acceptance testing: generates high-fidelity 3D environments, monitors safety parameters at runtime, and produces structured test reports. Now community-maintained as <em>DroneWorld</em> through the OSS-SLU open-source program.
</div>

<div class="site-research-gray" style="background:#f8fafc; padding:12px 16px; margin:5px 0; border-left:4px solid #94a3b8; border-radius:0 6px 6px 0; color:#111827;">
<strong>DroneWiS</strong><br>
CFD-based wind simulation built on DRV: uses OpenFOAM and a terrain scanning algorithm inside Unreal Engine to compute physics-accurate wind flows around buildings and terrain; wind stress-testing is unavailable in Gazebo or AirSim.
</div>

<div class="site-research-blue" style="background:#eef3fb; padding:12px 16px; margin:5px 0; border-left:4px solid #003DA5; border-radius:0 6px 6px 0; color:#111827;">
<strong>React-G</strong><br>
GNSS multipath simulation via ray casting in Unreal Engine with Google Maps 3D Tiles and Cesium, modeling Non-Line-of-Sight signal reflections in urban canyons to quantify navigation errors for sUAS.
</div>

<div class="site-research-gray" style="background:#f8fafc; padding:12px 16px; margin:5px 0; border-left:4px solid #94a3b8; border-radius:0 6px 6px 0; color:#111827;">
<strong>AutoSimTest</strong><br>
LLM-agent-driven framework that automates the generation, execution, and analysis of sUAS simulation test scenarios, reducing manual effort across the testing lifecycle.
</div>

<div style="text-align:center; margin:2.2em 0 1.8em;">
  <img src="{{ site.baseurl }}/images/photos/NASA_group_photo.PNG" alt="NASA ULI field validation: team and sUAS fleet at FAA-approved airfield" style="max-width:100%; border-radius:8px; box-shadow:0 2px 8px rgba(0,0,0,0.15);"/>
  <p style="font-size:0.82em; color:#6b7280; margin-top:0.5em;">NASA ULI field validation, testing sUAS at an FAA-approved airfield with the research team and drone fleet.</p>
</div>

---

## Background

I passed my PhD candidacy exam in 2025 and expect to graduate in May 2027. I hold an M.S. (GPA 3.95/4.0) and B.S. in Computer Science from SLU, and previously worked as an Assistant Engineer at Beijing VRV Software Corp Ltd. I also led an NSF-sponsored customer discovery study (interviewing 22 robotics professionals) to validate real-world demand for high-fidelity sUAS simulation tools.

---

## Lab & People

I work in the [UAVLab](https://github.com/UAVLab-SLU) at Saint Louis University, advised by [Dr. Ankit Agrawal](https://ankit.website/). Ankit's research spans software engineering, HCI, and safety-critical systems, with a particular focus on human-drone collaboration. It's a small, collaborative group and the work we do ends up at some pretty interesting places, from European conference venues to NASA airfields.

<div style="display:flex; gap:1em; flex-wrap:wrap; margin:1.4em 0;">
  <div style="flex:1; min-width:220px; text-align:center;">
    <img src="{{ site.baseurl }}/images/photos/SLU_lab_group_2.jpg" alt="Lab members in St. Louis" style="width:100%; border-radius:8px; box-shadow:0 2px 8px rgba(0,0,0,0.12);"/>
    <p style="font-size:0.8em; color:#6b7280; margin-top:0.4em;">Lab members on a summer afternoon in St. Louis.</p>
  </div>
  <div style="flex:1; min-width:220px; text-align:center;">
    <img src="{{ site.baseurl }}/images/photos/SLU_lab_group_1.jpg" alt="Lab group at the ice cream bar" style="width:100%; border-radius:8px; box-shadow:0 2px 8px rgba(0,0,0,0.12);"/>
    <p style="font-size:0.8em; color:#6b7280; margin-top:0.4em;">Post-deadline ice cream is a lab tradition.</p>
  </div>
</div>

A good chunk of my research involves validating simulation against reality, which means occasionally taking an anemometer to the field to record real wind conditions that DroneWiS needs to replicate.

<div style="text-align:center; margin:1.4em 0;">
  <img src="{{ site.baseurl }}/images/photos/wind_exp.png" alt="Measuring real wind speed for DroneWiS validation" style="max-width:380px; width:100%; border-radius:8px; box-shadow:0 2px 8px rgba(0,0,0,0.12);"/>
  <p style="font-size:0.8em; color:#6b7280; margin-top:0.4em;">Recording real-world wind measurements at SLU's athletic field for DroneWiS ground truth validation.</p>
</div>

### Collaborators

Beyond SLU, I've had the chance to work with some great people:

- **[Prof. Douglas Thain](https://www3.nd.edu/~dthain/), University of Notre Dame**: Doug leads the [Cooperative Computing Lab (CCL)](https://ccl.cse.nd.edu/) at Notre Dame, whose work on large-scale distributed systems complements our simulation infrastructure research. We've collaborated on scaling sUAS testing to city-scale missions (SADE-SIM).

- **Julian Gutierrez, NASA Langley Research Center**: Julian works in the Safety-Critical Avionics Systems Branch at Langley and provided real-world GNSS measurement data from flight experiments, which we used to validate React-G's multipath simulation against actual sUAS navigation error profiles.

<div style="text-align:center; margin:1.4em 0;">
  <img src="{{ site.baseurl }}/images/photos/ND.JPG" alt="Research visit to the University of Notre Dame" style="max-width:520px; width:100%; border-radius:8px; box-shadow:0 2px 8px rgba(0,0,0,0.12);"/>
  <p style="font-size:0.8em; color:#6b7280; margin-top:0.4em;">Research visit to Notre Dame, collaborating with Prof. Thain's group on multi-sUAS mission simulation.</p>
</div>

---

## Selected Publications

<div class="site-pub-row-blue" style="background:#eef3fb; padding:7px 14px; margin:3px 0; border-radius:4px; font-size:0.93em; color:#111827;">
B. Zhang, A. Putta, A. Agrawal. <strong>Advancing sUAS Simulation Testing in Realistic Windy Conditions.</strong> <em>IEEE Access</em>, 2026.
</div>
<div class="site-pub-row-white" style="background:#fff; padding:7px 14px; margin:3px 0; border-radius:4px; font-size:0.93em; color:#111827; border:1px solid #e8eef8;">
B. Zhang, J. Gutierrez, A. Agrawal. <strong>React-G: GNSS Signal Multipath Simulation Framework for small UAS.</strong> <em>IEEE/ION PLANS 2025.</em>
</div>
<div class="site-pub-row-blue" style="background:#eef3fb; padding:7px 14px; margin:3px 0; border-radius:4px; font-size:0.93em; color:#111827;">
V. S. A. Duvvuru, B. Zhang, M. Vierhauser, A. Agrawal. <strong>LLM-Agents Driven Automated Simulation Testing and Analysis of small UAS.</strong> <em>ICSE 2025.</em>
</div>
<div class="site-pub-row-white" style="background:#fff; padding:7px 14px; margin:3px 0; border-radius:4px; font-size:0.93em; color:#111827; border:1px solid #e8eef8;">
B. Zhang, A. Agrawal. <strong>DroneWiS: Automated Simulation Testing of small UAS in Realistic Windy Conditions.</strong> <em>ASE 2024.</em>
</div>
<div class="site-pub-row-blue" style="background:#eef3fb; padding:7px 14px; margin:3px 0; border-radius:4px; font-size:0.93em; color:#111827;">
B. Zhang, Y. Shivalingaiah, A. Agrawal. <strong>DroneReqValidator: Facilitating High Fidelity Simulation Testing for UAS Developers.</strong> <em>ASE 2023.</em>
</div>

<p style="margin-top:1em; font-size:0.93em;"><a href="/publications/">→ View all publications</a></p>
