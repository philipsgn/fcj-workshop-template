---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:
- Map model classification outputs to structured JSON entities.
- Wrap the AI model inside a RESTful API.
- Deploy the API via Amazon ECS (Elastic Container Service).

### Tasks for the Week:

| Day | Tasks |
| --- | --- |
| Mon | - Map bounding box outputs to logical fields (Seller Name, VAT Code, Created Date). <br> - Write regex fallback logic for common structures (e.g., Vietnam Tax ID). |
| Tue | - Build a fast RESTful API using FastAPI/Flask to serve inference. <br> - Implement POST endpoints accepting image files in multipart/form-data. |
| Wed | - Containerize the FastAPI application using the model weights synchronized from S3. <br> - Validate the Docker container works locally. |
| Thu | - Dive into Amazon ECS concepts: Task Definitions, Services, Clusters. <br> - Understand AWS Fargate architecture (serverless containers). |
| Fri | - **Practice:** <br>&emsp; + Push the API Docker image to ECR <br>&emsp; + Deploy an ECS Cluster using Fargate to host the inference API globally. |

### Week 6 Achievements:

- Built robust post-processing logic combining deep learning with regular expressions.
- Developed a production-grade FastAPI web service hosting AI inference.
- Deployed a highly scalable container architecture without managing EC2 instances via ECS Fargate.

