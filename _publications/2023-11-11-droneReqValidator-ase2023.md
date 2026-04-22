---
title: "DroneReqValidator: Facilitating High Fidelity Simulation Testing for Uncrewed Aerial Systems Developers"
collection: publications
category: conferences
permalink: /publication/2023-11-11-droneReqValidator-ase2023
excerpt: 'Presents DroneReqValidator (DRV), a comprehensive sUAS simulation ecosystem that automatically generates realistic environments, monitors drone activity against safety parameters, and produces detailed acceptance test reports. Demonstrated at ASE 2023.'
date: 2023-11-11
venue: '2023 38th IEEE/ACM International Conference on Automated Software Engineering (ASE)'
project_url: /portfolio/droneworld/
paperurl: 'https://ieeexplore.ieee.org/document/10298451/'
image: /images/drv/4droneCesiumGoogleAPI.gif
citation: 'B. Zhang, Y. Shivalingaiah, and A. Agrawal. (2023). &quot;DroneReqValidator: Facilitating High Fidelity Simulation Testing for Uncrewed Aerial Systems Developers.&quot; <i>2023 38th IEEE/ACM International Conference on Automated Software Engineering (ASE)</i>. pp. 2082–2085. DOI: 10.1109/ASE56229.2023.00011.'
---

**DroneReqValidator (DRV)** is a comprehensive drone simulation ecosystem that automatically creates realistic environments, monitors drone activity against predefined safety parameters, and produces detailed acceptance test reports for efficient debugging and analysis of drone software applications.

DRV employs a client-server architecture with a React-based frontend and a Python/Flask backend. It integrates Unreal Engine, Google Earth digital twin models, and AirSim APIs to automatically generate realistic 3D simulation environments. Key capabilities include:

- **Automatic Realistic Environment Generation**:four distinctive maps (Blocks, City Park, Chicago Scanning, Cesium) including ultra-realistic urban environments powered by Lumen lighting, Nanite, and real-time satellite scanning.
- **UAV Sensor Configuration**:per-drone specification of GPS, Camera, Lidar, Barometer, and Magnetometer sensors.
- **Automated Fuzzy Testing**:automatically manipulates environmental factors to explore operating boundaries.
- **Runtime Monitoring and Report Generation**:continuously collects sensor data and flags safety property violations with graphical analysis plots.

**Authors:** Bohan Zhang, Yashaswini Shivalingaiah, Ankit Agrawal

**Venue:** 38th IEEE/ACM International Conference on Automated Software Engineering (ASE 2023), Echternach, Luxembourg, November 11–15, 2023.

[Download paper](https://ieeexplore.ieee.org/document/10298451/)
