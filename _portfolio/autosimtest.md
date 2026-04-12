---
title: "AutoSimTest: LLM-Agent-Driven sUAS Simulation Testing"
excerpt: "A multi-LLM-agent framework that automates the full sUAS simulation testing pipeline — from scenario generation to flight log analysis — significantly reducing manual effort while improving test coverage."
collection: portfolio
---

## AutoSimTest: LLM-Agents Driven Automated Simulation Testing

**AutoSimTest** is a Large Language Model (LLM)-driven framework where multiple specialized AI agents collaborate to automate the end-to-end sUAS simulation testing process, from scenario design through execution to automated flight log analysis.

### Motivation

Despite the existence of sUAS simulation tools, the process of creating test scenarios, configuring simulation environments, generating mission plans, and interpreting results remains largely manual — requiring deep domain knowledge and significant time investment. AutoSimTest addresses all three pain points simultaneously.

### Multi-Agent Architecture

AutoSimTest operates across three coordinated phases using four specialized agents:

**Phase 1 — Scenario Blueprint Construction**
- **S-Agent (Scenario Generator)**: Takes high-level developer goals as input and uses Retrieval Augmented Generation (RAG) over a curated database of real-world sUAS incidents to produce scenario blueprints specifying environmental conditions, sUAS sensor specifications, mission objectives, and safety properties to test.

**Phase 2 — Scenario Specification and Execution**
- **Env-Agent (Environment Agent)**: Translates the S-Agent's environment description into a simulation configuration script (JSON/XML) for DRV/AirSim.
- **M-Agent (Mission Agent)**: Generates the sUAS mission execution script specifying flight tasks, waypoints, and mission modes.

**Phase 3 — Scenario Analysis**
- **Analytics-Agent**: Automatically analyzes flight logs to detect anomalous behavior, interpret telemetry data, and present interactive analysis reports to developers.

### Key Results

- Demonstrated capability across diverse sUAS types (PX4 and ArduPilot flight controllers)
- Significantly improves efficiency and scope of sUAS testing
- Reduces manual effort while enabling more varied and comprehensive scenario evaluations
- Evaluated by sUAS developers; perceived as valuable for both novice and expert users

### Links

- [ACM Digital Library (ICSE 2025)](https://dl.acm.org/doi/10.1109/ICSE55347.2025.00223)
- [Semantic Scholar](https://www.semanticscholar.org/paper/LLM-Agents-Driven-Automated-Simulation-Testing-and-Duvvuru-Zhang/54fefce853f9c73dd2b9b501e215df631027c42c)
