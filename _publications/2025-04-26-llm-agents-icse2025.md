---
title: "LLM-Agents Driven Automated Simulation Testing and Analysis of small Uncrewed Aerial Systems"
collection: publications
category: conferences
permalink: /publication/2025-04-26-llm-agents-icse2025
excerpt: 'Proposes AutoSimTest, a multi-LLM-agent framework that automates the full sUAS simulation testing pipeline: scenario blueprint construction, scenario specification and execution, and automated flight log analysis. Significantly reduces manual effort while enabling more comprehensive and varied scenario evaluations.'
date: 2025-04-26
venue: '2025 IEEE/ACM 47th International Conference on Software Engineering (ICSE)'
project_url: /portfolio/autosimtest/
paperurl: 'https://dl.acm.org/doi/10.1109/ICSE55347.2025.00223'
video: /video/agent.mp4
demo_url: https://www.flightassistant.app/
citation: 'V. S. A. Duvvuru, B. Zhang, M. Vierhauser, and A. Agrawal. (2025). &quot;LLM-Agents Driven Automated Simulation Testing and Analysis of small Uncrewed Aerial Systems.&quot; <i>Proceedings of the IEEE/ACM 47th International Conference on Software Engineering (ICSE &apos;25)</i>. pp. 385–397. DOI: 10.1109/ICSE55347.2025.00223.'
---

Thorough simulation testing is crucial for validating sUAS behavior across diverse scenarios, but the entire process of creating, executing, and analyzing tests remains largely manual. **AutoSimTest** addresses this with a Large Language Model (LLM)-driven framework where multiple specialized agents collaborate to automate sUAS simulation testing end-to-end.

The framework operates in three phases:

1. **Scenario Blueprint Construction**: The *S-Agent* uses Retrieval Augmented Generation (RAG) over real-world sUAS incident databases to generate scenario blueprints specifying environmental conditions, mission objectives, and safety test properties.
2. **Scenario Specification and Execution**: The *Env-Agent* translates blueprints into simulation configuration scripts; the *M-Agent* generates sUAS mission execution scripts. Both leverage DRV and AirSim APIs.
3. **Scenario Analysis**: The *Analytics-Agent* automatically analyzes flight logs, identifies anomalous behavior, and presents interactive analysis results to developers.

Extensive experiments demonstrated that AutoSimTest significantly improves efficiency and scope of sUAS testing, reducing manual effort while enabling more comprehensive scenario evaluations.

**Authors:** Venkata Sai Aswath Duvvuru, Bohan Zhang, Michael Vierhauser, Ankit Agrawal

**Venue:** IEEE/ACM 47th International Conference on Software Engineering (ICSE 2025), Ottawa, Canada, April 26 – May 2, 2025.

[Download paper](https://dl.acm.org/doi/10.1109/ICSE55347.2025.00223)
