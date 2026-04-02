---
title: "Week 8 Worklog"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:
- Implement asynchronous batch processing for mass invoice uploads.
- Integrate AWS SQS (Simple Queue Service) into the pipeline.
- Conduct rigorous F1-Score evaluation and re-tuning.

### Tasks for the Week:

| Day | Tasks |
| --- | --- |
| Mon | - Study architectural challenges of processing 10,000 invoices concurrently (Timeout issues, API drops). <br> - Learn Amazon SQS messaging architecture. |
| Tue | - Provision an SQS Standard Queue. <br> - Write a producer script (pushing S3 image URLs to SQS) and a consumer script (reading from SQS -> passing to OCR Model -> RDS). |
| Wed | - Conduct rigorous formal evaluation of the LayoutLM model on the Test Dataset. <br> - Calculate Token-level Precision, Recall, and F1-score. |
| Thu | - Perform hyperparameter tuning based on false negatives/positives. <br> - Retrain and hot-swap the model in ECS. |
| Fri | - **Practice:** <br>&emsp; + Push 200 invoice requests into the SQS queue <br>&emsp; + Boot up Multiple ECS tasks to consume the queue in parallel and measure processing throughput. |

### Week 8 Achievements:

- Transitioned the system from synchronous bottlenecks to a decoupled, asynchronous, scalable architecture.
- Mastered AWS SQS integrations for job scheduling and parallel AI consumption.
- Achieved targeted precision metrics through data-driven hyperparameter iteration.

