---
title: "DroneReqValidator / DroneWorld"
excerpt: "Open-source sUAS simulation ecosystem for requirements-driven safety testing. Originally developed as my primary PhD research project and now maintained by SLU undergraduates through the OSS-SLU program.<br/><img src='{{ site.baseurl }}/images/drv/4droneCesiumGoogleAPI.png' style='max-width:480px; margin-top:8px;'>"
collection: portfolio
image: /images/drv/4droneCesiumGoogleAPI.gif
---

## DroneReqValidator (DRV) / DroneWorld

**DroneReqValidator (DRV)** is a comprehensive drone simulation ecosystem that automatically creates high-fidelity 3D environments, monitors drone activity against predefined safety parameters, and produces detailed acceptance test reports for sUAS software developers.

---

### Demo Video

<iframe width="560" height="315" src="https://www.youtube.com/embed/Fd9ft55gbO8" title="DRV Demo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---

### Four Drones in a Cesium Real-World Environment

![Four drones flying in a Cesium/Google API digital twin environment]({{ site.baseurl }}/images/drv/4droneCesiumGoogleAPI.gif)

*Four sUAS simultaneously conducting a mission in DRV's Cesium-powered real-world digital twin, with live satellite terrain streaming via Google Maps API.*

---

### User Interface: Three-Step Configuration Wizard

DRV guides developers through a three-step wizard to fully configure a simulation test:

**Step 1: Environment Configuration**

![DRV environment configuration page]({{ site.baseurl }}/images/drv/webpage1env.png)

*Configure geographic location, weather conditions (wind speed/direction, precipitation), time of day, and GPS signal interference parameters.*

**Step 2: Vehicle (sUAS) Configuration**

![DRV vehicle and sensor configuration page]({{ site.baseurl }}/images/drv/webpage_p2_veh.png)

*Specify the number of sUAS to deploy, sensor loadouts (GPS, Camera, Lidar, Barometer, Magnetometer), and individual home geolocations.*

**Step 3: Safety Test Property Configuration**

![DRV test property configuration page]({{ site.baseurl }}/images/drv/webpage_p3_tests.png)

*Define safety test properties: maximum flight path deviation, minimum separation distances, no-fly zones, safe landing requirements, and collision detection thresholds.*

---

### Acceptance Test Report: Pass/Fail Analysis

![DRV acceptance test report showing pass and fail cases for two sUAS]({{ site.baseurl }}/images/drv/results.png)

*Automatically generated acceptance test report. sUAV 2 (left, green): **PASS**: deviation within 15 m threshold. sUAV 1 (right, red): **FAIL**: deviation exceeds 15 m. Each report includes 3D planned-vs-actual trajectory plots for every sUAS in the mission.*

---

### Background & Impact

I initiated DRV as the cornerstone of my PhD research, sponsored by the [NASA University Leadership Initiative (ULI)](https://www.nasa.gov/directorates/armd/tacp/ui/uli/). The goal was to bridge the gap between high-level safety requirements and practical simulation-based validation for sUAS developers.

DRV has since grown into a community-driven open-source project under the name **DroneWorld**, actively developed by undergraduate contributors at SLU through the [OSS-SLU](https://github.com/oss-slu/DroneWorld) program, with **4 official releases**, **52+ branches**, and contributions from dozens of students.

---

### Links

- [OSS-SLU DroneWorld Repository](https://github.com/oss-slu/DroneWorld)
- [Original UAVLab-SLU Repository](https://github.com/UAVLab-SLU/DRV_public)
- [ASE 2023 Paper](https://ieeexplore.ieee.org/document/10298451/)
- [RE 2023 Paper](https://ieeexplore.ieee.org/document/10260819/)
- [ASE 2024 Paper (DroneWiS)](https://dl.acm.org/doi/10.1145/3691620.3695351)
