---
title: "Week 4 Worklog"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:
- Learn Docker containerization and Amazon ECR.
- Establish strong ground truth bounding boxes for model training.
- Automate data augmentation techniques to prevent overfitting.

### Tasks for the Week:

| Day | Tasks |
| --- | --- |
| Mon | - Study Docker principles, creating Dockerfiles for Python environments. <br> - Learn Amazon ECR (Elastic Container Registry). |
| Tue | - Set up an open-source data annotation tool (e.g., Label Studio) on EC2. <br> - Define the entity schema (Seller, Tax ID, Date, Amount, etc.). |
| Wed | - Annotate 200+ complex Vietnamese invoices manually to create a robust Ground Truth benchmark. <br> - Export datasets to standard JSON format. |
| Thu | - Write scripts for Data Augmentation (random crops, varying brightness/contrast, simulating shadows). <br> - Sync the augmented dataset back to S3. |
| Fri | - **Practice:** <br>&emsp; + Containerize the training pipeline into a Docker image <br>&emsp; + Authenticate and push the Docker image to Amazon ECR. |

### Week 4 Achievements:

- Gained practical experience creating and managing Docker images via Amazon ECR.
- Produced a high-quality annotated dataset, overcoming the cold-start problem in ML.
- Successfully wrote custom data augmentation pipelines to enhance model robustness.

