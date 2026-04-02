---
title: "Week 11 Worklog"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:
- Engineer mathematical cross-validation rules to guarantee data schema integrity.
- Develop confidence scoring logic to flag manual reviews.
- Secure cloud credentials using AWS Systems Manager / Secrets Manager.

### Tasks for the Week:

| Day | Tasks |
| --- | --- |
| Mon | - Implement the 'Math Validation' layer: Total Amount must strictly equal (Unit Price x Quantity) + VAT. <br> - Formulate discrepancy fallback policies. |
| Tue | - Build a robust 'Confidence Score' for each extracted entity out of 100%. <br> - Append colored status metadata (Green/Yellow/Red) based on the score threshold. |
| Wed | - Audit current security architecture: Remove any hardcoded LLM API Keys or RDS Database passwords from source code. |
| Thu | - Learn AWS Systems Manager (Parameter Store) and AWS Secrets Manager. <br> - Move all sensitive environment variables into Secrets Manager. |
| Fri | - **Practice:** <br>&emsp; + Refactor the ECS Task definition to pull secrets securely by referencing Secrets Manager ARNs <br>&emsp; + Test ECS reboot and ensure the application boots without hardcoded keys. |

### Week 11 Achievements:

- Brought the system error tolerance to production standards with comprehensive mathematical checks.
- Seamlessly integrated a Human-in-the-loop verification workflow through confidence tracking.
- Acheived enterprise-level security for sensitive backend credentials using AWS Secrets Manager.

