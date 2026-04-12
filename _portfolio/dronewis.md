---
title: "DroneWiS — CFD-Based Wind Simulation for sUAS"
excerpt: "A Computational Fluid Dynamics pipeline integrated into DRV that automatically scans 3D environments, computes realistic wind fields using OpenFOAM, and exposes them to sUAS simulation for physics-accurate wind testing.<br/><img src='/mywebsite/images/dronewis/phase3_windGen.png' style='max-width:480px; margin-top:8px;'>"
collection: portfolio
---

## DroneWiS — Drone Wind Simulation

**DroneWiS** is DRV 2.0's core innovation: a fully automated Computational Fluid Dynamics (CFD) pipeline that computes realistic wind flow fields around real-world terrain and urban structures, then feeds them into sUAS simulation for physics-accurate wind stress testing.

Existing tools (Gazebo, AirSim) model wind as simple constant or stochastic vectors — they cannot capture how wind interacts with buildings, trees, or uneven ground. DroneWiS closes this gap.

---

### Three-Phase Pipeline

#### Phase 1 — Terrain Scanning

![Terrain scanning algorithm generating a voxel grid from the 3D environment](/mywebsite/images/dronewis/phase1terrain_gen.png)

*The terrain scanning algorithm overlays a volumetric voxel grid on the Unreal Engine 3D environment. Each cell is tested for obstruction via ray casting to build a binary occupancy map — identifying where wind can flow freely versus where objects block it.*

---

#### Phase 2 — Voxelization & CFD Input Preparation

![Voxelized terrain representation used as input to OpenFOAM](/mywebsite/images/dronewis/phase2_voxelization.png)

*The occupancy map is converted into an OpenFOAM-compatible mesh. DroneWiS automatically configures OpenFOAM boundary conditions according to user-specified wind parameters: direction, speed, type (uniform, turbulent, or multi-source).*

---

#### Phase 3 — Wind Simulation & Runtime Injection

**Wind field generation:**

![OpenFOAM wind field computed around terrain and buildings](/mywebsite/images/dronewis/phase3_windGen.png)

*OpenFOAM computes the full 3D wind vector field. Colors indicate wind speed (blue = low, red = high). Wind accelerates and deflects around building edges and through urban canyons — effects invisible to simpler models.*

**Simulation and flight analysis:**

![Phase 3 simulation execution and analysis dashboard](/mywebsite/images/dronewis/phase3_sim_and_analysis.png)

*The computed wind vectors are injected into the DRV simulation at runtime. The sUAS executes its mission while the monitoring system collects telemetry and compares actual trajectory against planned path.*

---

### Evaluation Results

#### RQ2 — Wind Field Fidelity

![DroneWiS vs AirSim wind field comparison with sUAS trajectory](/mywebsite/images/dronewis/rq2_copy.png)

*Left: 3D wind field computed by DroneWiS (OpenFOAM) showing directional vectors around voxelized terrain — capturing complex turbulence and wake effects. Right: sUAS trajectory comparison between DroneWiS (red, realistic wind) and AirSim (blue dashed, simplified wind). The DroneWiS trajectory shows realistic wind-induced drift consistent with real-world physics.*

#### RQ3 — sUAS Performance Under Realistic Wind Conditions

![RQ3 part 1 - sUAS mission results under DroneWiS wind](/mywebsite/images/dronewis/rq3p1_wis.png)

![RQ3 full results comparison](/mywebsite/images/dronewis/rq3p2_full.png)

*Evaluation of sUAS mission success rates and safety property violations under DroneWiS-generated wind versus simplified wind models. DroneWiS exposes safety violations undetectable by existing simulation tools.*

---

### Links

- [ASE 2024 Paper](https://dl.acm.org/doi/10.1145/3691620.3695351)
- [DroneWorld Repository](https://github.com/oss-slu/DroneWorld)
- [Demo Video](https://youtu.be/khBHEBST8Wc)
