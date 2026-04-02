---
title: "Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1. </b> "
---

Below is the worklog detailing my 12-week internship as an AI Developer, focusing on the research, development, and optimization of the Invoice Information Extraction (Invoice OCR) system, alongside mastering fundamental AWS Cloud services.

The internship process can be analyzed through four main phases:
1. **Phase 1 (Week 1-4): AWS Foundations & AI Prep.** Establishing cloud environments (EC2, S3, Lambda) and evaluating OCR baselines (Amazon Textract).
2. **Phase 2 (Week 5-8): Core Model & Cloud Integration.** Training layout-aware models, deploying via Amazon ECS, and managing data with RDS/SQS.
3. **Phase 3 (Week 9-11): LLM Integration & Optimization.** Integrating LLM (Gemini/Bedrock), monitoring with CloudWatch, and securing API Keys.
4. **Phase 4 (Week 12): Resilience & Finalization.** Finalizing the fallback architecture and ensuring production scaling.

**Week 1:** [AWS Foundations & Environment. Learning IAM, basic VPC, and setting up EC2 instances for Jupyter/PyTorch OCR research.](1.1-week1/)

**Week 2:** [Cloud Storage & Baseline OCR. Exploring Amazon S3 for invoice datasets and benchmarking Amazon Textract vs Tesseract.](1.2-week2/)

**Week 3:** [Serverless Compute & Data Pipeline. Utilizing AWS Lambda for automated image preprocessing (Deskew, Binarization) via S3 triggers.](1.3-week3/)

**Week 4:** [Containerization & Annotation. Packaging environments with Docker, using Amazon ECR, and augmenting data for OCR algorithms.](1.4-week4/)

**Week 5:** [Model Training & Compute Scaling. Training layout-aware AI models and exploring GPU-optimized EC2 instances/SageMaker for faster training.](1.5-week5/)

**Week 6:** [API Development & Entity Mapping. Building logic for extracting key points and deploying the OCR API via Amazon ECS/Fargate.](1.6-week6/)

**Week 7:** [Database Storage & Table Extraction. Solving line item extraction and storing structured JSON responses to Amazon RDS/DynamoDB.](1.7-week7/)

**Week 8:** [Queue Systems & Model Evaluation. Integrating AWS SQS for asynchronous invoice processing queues and evaluating model F1-score.](1.8-week8/)

**Week 9:** [LLM Integration & Prompt Engineering. Researching and integrating Large Language Models (Gemini/Amazon Bedrock) as OCR fallbacks.](1.9-week9/)

**Week 10:** [Performance Tuning & Monitoring. Optimizing inference latency and setting up Amazon CloudWatch metrics/alarms for the OCR API.](1.10-week10/)

**Week 11:** [Security & Confidence Validation. Implementing Math Validation and securing LLM API Keys using AWS Secrets Manager/Parameter Store.](1.11-week11/)

**Week 12:** [System Resilience. Finalizing Edge Case handling, the AI Fallback logic, and completing the production-ready SmartInvoice pipeline.](1.12-week12/)
