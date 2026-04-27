# Final Report Package

This repository now contains a full academic delivery package for the AI-Based Web Application Firewall project. The package has been rewritten to describe the implemented system as it actually exists in the repository, with chapter content grounded in three primary evidence sources:

- [README.md](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/README.md)
- [system_architecture.md](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/system_architecture.md)
- [reports](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/reports)

## Abstract

This project implements a hybrid web application firewall that combines deterministic rules, behavioral feature extraction, anomaly-aware scoring, targeted mitigation, persistent storage, and an analyst-facing React command center. The system supports both a local embedded mode and a production-style separated deployment using Flask, React, PostgreSQL, Redis, Docker, and Nginx. Experimental results show that the rule engine is highly effective on the current labeled datasets, while the Isolation Forest anomaly model still introduces false positives and therefore does not yet outperform the rules-only baseline. The project nevertheless demonstrates a complete research workflow: request capture, storage, labeling, export, training, evaluation, benchmark measurement, administration, and deployment.

## Chapters

1. [Chapter 1: Introduction](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/chapters/chapter_1_introduction.md)
2. [Chapter 2: Literature Review](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/chapters/chapter_2_literature_review.md)
3. [Chapter 3: Requirements and Analysis](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/chapters/chapter_3_requirements_analysis.md)
4. [Chapter 4: Methodology and Design](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/chapters/chapter_4_methodology_design.md)
5. [Chapter 5: Implementation and Results](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/chapters/chapter_5_implementation_results.md)
6. [Chapter 6: Discussion and Conclusion](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/chapters/chapter_6_discussion_conclusion.md)
7. [Appendices](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/chapters/appendices.md)

## List of Figures

- Figure 3.1. Use case diagram for the implemented AI-Based WAF control plane and data plane.
- Figure 3.2. Simplified class and module view of the implemented security pipeline.
- Figure 3.3. Actual request-processing flow based on the current `handle_security_pipeline()` implementation.
- Figure 3.4. Sequence diagram for the implemented allow, inspect, and block paths.
- Figure 3.5. Activity view showing the runtime request path and the analyst/admin control loop.
- Figure 3.6. Entity relationship diagram for the repository-backed persistence layer.
- Figure 3.7. Representative capstone delivery plan reconstructed from the completed repository work.
- Figure 4.1. High-level component view.
- Figure 4.2. Request processing sequence.
- Figure 4.3. Control-plane and analyst workflow.
- Figure 4.4. ML and data lifecycle.
- Figure 4.5. Deployment topology.

## List of Tables

- Table 3.1. Functional requirements aligned to the implemented repository.
- Table 3.2. Non-functional requirements and current status.
- Table 3.3. Software stack derived from the repository.
- Table 3.4. Runtime context grounded in repository evidence.
- Table 3.5. System analysis summary.
- Table 3.6. Representative delivery phases aligned to the completed system.
- Table 3.7. Validation layers and evidence.
- Table 4.1. Dataset summary used by the current evaluation workflow.
- Table 5.1. Detection results on labeled telemetry.
- Table 5.2. Detection results on prepared public data.
- Table 5.3. Runtime benchmark results.
- Table 5.4. Assessment against success criteria.

## Key generated evidence

- Academic metrics summary: [academic_results.md](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/reports/academic_results.md)
- Machine-readable metrics: [academic_results.json](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/reports/academic_results.json)
- Local benchmark: [benchmark_summary_local.json](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/reports/benchmark_summary_local.json)
- Docker benchmark: [benchmark_summary.json](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/reports/benchmark_summary.json)
- Inspection benchmark local: [benchmark_inspect_local.json](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/reports/benchmark_inspect_local.json)
- Inspection benchmark docker: [benchmark_inspect_docker.json](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/reports/benchmark_inspect_docker.json)
- Rate-limit stress evidence: [rate_limit_stress.json](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/reports/rate_limit_stress.json)
- Automated tests evidence: [test_results.txt](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/reports/test_results.txt)
- Health snapshots: [health_local.json](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/reports/health_local.json) and [health_docker.json](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/reports/health_docker.json)

## Architecture and presentation assets

- Architecture diagrams: [system_architecture.md](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/system_architecture.md)
- Presentation deck: [presentation_deck.md](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/presentation_deck.md)
- References: [references.md](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/references.md)

## Reproducibility

To regenerate the academic metrics package:

```powershell
cd C:\Users\tamat\OneDrive\Desktop\wafai\waf_project
python scripts\generate_academic_results.py
```

To regenerate tests and benchmarks, follow the workflow in [appendices.md](C:/Users/tamat/OneDrive/Desktop/wafai/waf_project/docs/chapters/appendices.md).
