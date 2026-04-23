---
title: "DroneWiS: CFD-Based Wind Simulation for sUAS"
excerpt: "A Computational Fluid Dynamics pipeline integrated into DRV that automatically scans 3D environments, computes realistic wind fields using OpenFOAM, and exposes them to sUAS simulation for physics-accurate wind testing.<br/><img src='{{ site.baseurl }}/images/dronewis/phase3_windGen.png' style='max-width:480px; margin-top:8px;'>"
collection: portfolio
image: /images/dronewis/phase3_windGen.png
---

## DroneWiS: Drone Wind Simulation

<div style="background:#fffbeb; border-left:4px solid #d97706; padding:12px 16px; border-radius:0 6px 6px 0; margin-bottom:1.4em; color:#111827;">
<strong>Award: 5th Place Individual Poster</strong> — First Annual NASA imaginAviation University Poster Session, February 28, 2024.<br>
The early version of this work (titled <em>RealWindDroneSim / RWDS</em>) was presented at this NASA-sponsored virtual poster session and received a 5th place individual award among university participants.<br>
<a href="{{ site.baseurl }}/files/imaginaviation2024_award_certificate.pdf" target="_blank">View award certificate</a> &nbsp;|&nbsp; <a href="{{ site.baseurl }}/files/rwds_imaginaviation2024_poster.pdf" target="_blank">View original poster</a>
</div>

**DroneWiS** is DRV 2.0's core innovation: a fully automated Computational Fluid Dynamics (CFD) pipeline that computes realistic wind flow fields around real-world terrain and urban structures, then feeds them into sUAS simulation for physics-accurate wind stress testing.

Existing tools (Gazebo, AirSim) model wind as simple constant or stochastic vectors; they cannot capture how wind interacts with buildings, trees, or uneven ground. DroneWiS closes this gap.

---

### Three-Phase Pipeline

#### Phase 1: Terrain Scanning

![Terrain scanning algorithm generating a voxel grid from the 3D environment]({{ site.baseurl }}/images/dronewis/phase1terrain_gen.png)

*The terrain scanning algorithm overlays a volumetric voxel grid on the Unreal Engine 3D environment. Each cell is tested for obstruction via ray casting to build a binary occupancy map, identifying where wind can flow freely versus where objects block it.*

---

#### Phase 2: Voxelization and CFD Input Preparation

![Voxelized terrain representation used as input to OpenFOAM]({{ site.baseurl }}/images/dronewis/phase2_voxelization.png)

*The occupancy map is converted into an OpenFOAM-compatible mesh. DroneWiS automatically configures OpenFOAM boundary conditions according to user-specified wind parameters: direction, speed, type (uniform, turbulent, or multi-source).*

---

#### Phase 3: Wind Simulation and Runtime Injection

**Wind field generation:**

![OpenFOAM wind field computed around terrain and buildings]({{ site.baseurl }}/images/dronewis/phase3_windGen.png)

*OpenFOAM computes the full 3D wind vector field. Colors indicate wind speed (blue = low, red = high). Wind accelerates and deflects around building edges and through urban canyons; these effects are invisible to simpler models.*

**Simulation and flight analysis:**

![Phase 3 simulation execution and analysis dashboard]({{ site.baseurl }}/images/dronewis/phase3_sim_and_analysis.png)

*The computed wind vectors are injected into the DRV simulation at runtime. The sUAS executes its mission while the monitoring system collects telemetry and compares actual trajectory against planned path.*

---

### Evaluation Results

#### RQ2: Wind Field Fidelity

![DroneWiS vs AirSim wind field comparison with sUAS trajectory]({{ site.baseurl }}/images/dronewis/rq2_copy.png)

*Left: 3D wind field computed by DroneWiS (OpenFOAM) showing directional vectors around voxelized terrain, capturing complex turbulence and wake effects. Right: sUAS trajectory comparison between DroneWiS (red, realistic wind) and AirSim (blue dashed, simplified wind). The DroneWiS trajectory shows realistic wind-induced drift consistent with real-world physics.*

#### RQ3: sUAS Performance Under Realistic Wind Conditions

![RQ3 part 1 - sUAS mission results under DroneWiS wind]({{ site.baseurl }}/images/dronewis/rq3p1_wis.png)

![RQ3 full results comparison]({{ site.baseurl }}/images/dronewis/rq3p2_full.png)

*Evaluation of sUAS mission success rates and safety property violations under DroneWiS-generated wind versus simplified wind models. DroneWiS exposes safety violations undetectable by existing simulation tools.*

---

### Links

- [ASE 2024 Paper](https://dl.acm.org/doi/10.1145/3691620.3695351)
- [DroneWorld Repository](https://github.com/oss-slu/DroneWorld)
- [Demo Video](https://youtu.be/khBHEBST8Wc)
