---
title: "AutonomyLens: A Self-Evolving Simulation-Based Testing Loop for Autonomous Systems"
collection: publications
category: workshops
permalink: /publication/2026-04-13-autonomylens-fse2026
excerpt: 'Introduces AutonomyLens, a self-evolving testing framework that uses LLM-driven agents to continuously generate, execute, and refine simulation-based tests for autonomous systems, closing the loop between test generation and failure analysis.'
date: 2026-04-13
venue: '2nd International Workshop on Software Engineering for Engineering Simulations (SE4ES), co-located with FSE 2026'
paperurl: 'https://arxiv.org/abs/2604.11672'
image: /images/abs_picture/AutonomyLens.png
citation: 'A. Agrawal, J. Garapati, and B. Zhang. (2026). &quot;AutonomyLens: A Self-Evolving Simulation-Based Testing Loop for Autonomous Systems.&quot; <i>Proceedings of the 2nd International Workshop on Software Engineering for Engineering Simulations (SE4ES &apos;26)</i>, co-located with FSE 2026.'
---

Testing autonomous systems is inherently difficult: the space of possible failure scenarios is vast, and hand-crafted test suites quickly become stale as system capabilities evolve. **AutonomyLens** addresses this by introducing a self-evolving testing loop powered by LLM-driven agents that automatically generate, execute, and refine simulation-based tests in response to observed system behavior.

**Key contributions:**
- Self-evolving test generation loop that adapts based on failure history and coverage gaps
- LLM agent pipeline for translating high-level operational requirements into executable simulation scenarios
- Automated failure analysis that distills simulation results into actionable test refinement signals
- Evaluation on sUAS autonomous mission scenarios demonstrating improved fault detection over static test suites

**Authors:** Ankit Agrawal, Jithin Garapati, Bohan Zhang

**Venue:** 2nd International Workshop on Software Engineering for Engineering Simulations (SE4ES '26), co-located with the 34th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (FSE '26), July 2026.

[Preprint](https://arxiv.org/abs/2604.11672)
