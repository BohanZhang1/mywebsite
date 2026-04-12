---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* **PhD in Computer Science**, Saint Louis University, St. Louis, MO — *Expected May 2027*
  * Focus: High-Fidelity UAV Simulation
  * Tuition fully sponsored by NASA University Leadership Initiative (ULI)
  * Passed candidacy exam: 2025
* **M.S. in Computer Science**, Saint Louis University, St. Louis, MO — *Spring 2024 (GPA: 3.95/4.0)*
* **B.S. in Computer Science**, Saint Louis University, St. Louis, MO — *Spring 2021 (GPA: 3.46/4.0)*

Research Experience
======
* **Doctoral Student / Graduate Research Assistant** — Saint Louis University *(Fall 2022 – Present)*
  * Developed **DroneReqValidator (DRV)**, an automated sUAS testing framework that generates high-fidelity 3D dynamic environments and monitors UAV safety parameters against system-level requirements.
  * Designed **DroneWiS**, a CFD-based wind simulation system (using OpenFOAM + Unreal Engine) that automatically computes realistic wind flows around terrain and buildings for sUAS evaluation.
  * Developed **React-G**, a GNSS multipath simulation framework using Unreal Engine ray casting, Google Maps 3D Tiles, and Cesium for Unreal to quantify navigation errors in dense urban environments.
  * Co-developed **AutoSimTest**, an LLM-agent-driven framework (Multi-Agent: S-Agent, Env-Agent, M-Agent, Analytics-Agent) that automates end-to-end sUAS simulation test scenario generation and analysis.
  * Led an NSF-sponsored I-Corps customer discovery initiative, conducting 22 interviews with robotics industry professionals to validate commercial demand for high-fidelity sUAS simulation tools.
  * Led the development of a DSL-driven framework for procedurally generating diverse environments with dynamic AI agents and trigger-based behaviors for repeatable sUAS testing.

Industry Experience
======
* **Assistant Engineer Intern** — Beijing VRV Software Corp Ltd, Xi'an Branch, China *(Fall 2021 – Summer 2022)*
  * Contributed to front-end and back-end development; implemented testing to ensure reliability of a large-scale enterprise software project.
  * Designed and developed a secure file encryption/decryption application with a graphical user interface in Java.

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Skills
======
* **Simulation & Game Engines:** Unreal Engine 5, AirSim, Gazebo
* **Programming:** Python, JavaScript, Java, C++
* **CFD & Scientific Computing:** OpenFOAM, Computational Fluid Dynamics
* **Web Development:** React, Flask, REST APIs, Docker
* **Research Areas:** sUAS/UAV Safety, Requirements Engineering, Automated Testing, GNSS Navigation, LLM Agents
* **Languages:** English (native/bilingual), Chinese (native/bilingual), Japanese (elementary)

Honors and Awards
======
* **Alpha Sigma Nu Honor Society** — *Fall 2024*
  * National Jesuit honor society; recognized for outstanding academic achievement and leadership.
* **NASA imaginAviation University Poster Individual Award — 5th Place** — *Spring 2024*
  * First Annual NASA imaginAviation University Poster Session; awarded for *RealWindDroneSim (RWDS)*.
* **$10,000 Global Graduate Scholar Award** — *Fall 2022 – Spring 2024*
  * Recognized for consistent academic excellence at Saint Louis University.
* **$5,000 James G. Costigan Endowed Scholarship** — *Spring 2021*
  * Granted by Saint Louis University in recognition of outstanding scholarly performance.
* **NASA University Leadership Initiative (ULI) Scholarship** — *Fall 2022 – Present*
  * Full PhD tuition sponsorship for exceptional academic and research contributions.

Service
======
* **Peer Reviewer**, IEEE International Conference on Robotics and Automation (ICRA 2026)
