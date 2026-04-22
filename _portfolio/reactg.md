---
title: "React-G: GNSS Multipath Simulation Framework"
excerpt: "A simulation framework using Unreal Engine ray casting, Google Maps 3D Tiles, and Cesium for Unreal to model GNSS multipath signal errors in urban environments, validated against real NASA NavQ hardware measurements.<br/><img src='{{ site.baseurl }}/images/reactg/react-g-overview.png' style='max-width:480px; margin-top:8px;'>"
collection: portfolio
image: /images/reactg/react-g-overview.png
---

## React-G: Reflective Environment Augmented Coordinates Tracking of GNSS

**React-G** is a simulation framework that approximates GNSS multipath signal behaviors in complex urban environments for sUAS. It uses Unreal Engine ray casting with Google Maps 3D Tiles and Cesium for Unreal to model how signals reflect off buildings and glass, causing the NLOS errors that degrade sUAS navigation accuracy in dense urban settings.

---

### Framework Overview

![React-G ray casting visualization in an urban environment]({{ site.baseurl }}/images/reactg/react-g-overview.png)

*React-G's ray casting approach for GNSS signal path simulation. **Green lines**: direct Line-of-Sight (LOS) paths (reliable signals). **Orange lines**: potential reflected NLOS paths (cause positioning errors). **Blue lines**: blocked LOS paths (signal fully obstructed).*

---

### System Architecture

![React-G system architecture diagram]({{ site.baseurl }}/images/reactg/react-g-architecture.png)

*React-G's three-phase architecture: (1) **Configuration**: environment settings, satellite list, fidelity parameters; (2) **GNSS Simulation**: environment initialization via Cesium + Google Maps, LOS calculation, ray-traced NLOS multipath computation; (3) **Processing and Analysis**: material reflectivity filtering, output of LOS/NLOS path data.*

---

### Signal Path Visualization

![React-G merged visualization of LOS and NLOS signal paths across urban environment]({{ site.baseurl }}/images/reactg/react-g-merged.png)

*Combined visualization of all simulated signal paths. The framework computes both direct paths and reflected paths accounting for surface material properties (glass, concrete, metal), enabling identification of high-interference zones for sUAS mission planning.*

---

### Real-World Validation: Two Environments

#### Brick Building (Low Reflectivity)

| Real Environment | React-G Simulation |
|:---:|:---:|
| ![Brick building photo]({{ site.baseurl }}/images/reactg/react-g-brick.png) | ![React-G simulation of brick building]({{ site.baseurl }}/images/reactg/react-g-brick-sim.png) |

*Brick-facade building with low surface reflectivity. React-G models reduced NLOS signal scattering characteristic of matte, absorptive surfaces.*

---

#### Glass/Modern Building (High Reflectivity)

| Real Environment | React-G Simulation |
|:---:|:---:|
| ![Modern glass building photo]({{ site.baseurl }}/images/reactg/react-g-spring.png) | ![React-G simulation of glass building with dense NLOS reflections]({{ site.baseurl }}/images/reactg/react-g-spring-sim.png) |

*Modern building with large glass panels, high reflectivity surfaces generating dense NLOS multipath signals that significantly degrade GNSS accuracy.*

---

### Real-World Validation Hardware

![NASA NavQ GNSS receiver testbed: SparkFun u-blox board with GNSS antenna on leveled platform]({{ site.baseurl }}/images/reactg/navq-hardware.jpg)

*React-G's real-world validation testbed: a SparkFun u-blox GNSS receiver with an external antenna, mounted on a leveled platform, built as part of this research. Real-world GNSS measurements collected with this setup were compared against React-G's simulated predictions, confirming the framework's ability to approximate real LOS/NLOS behavior. **Julian Gutierrez** at NASA Langley Research Center contributed real-world GNSS reference data for validation comparison.*

---

### Links

- [IEEE Xplore (PLANS 2025)](https://ieeexplore.ieee.org/document/11028333/)
- [NASA NTRS Record](https://ntrs.nasa.gov/citations/20250003844)
