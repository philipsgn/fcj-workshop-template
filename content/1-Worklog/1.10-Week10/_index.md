---
title: "Week 10 Worklog"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:
- Optimize deep learning models for faster inference (Quantization).
- Set up Amazon CloudWatch for live operational metrics.
- Identify and resolve latency bottlenecks.

### Tasks for the Week:

| Day | Tasks |
| --- | --- |
| Mon | - Assess current API response times (Latency ~3-5s per page). <br> - Research ONNX runtime and FP16/INT8 Quantization to compress the model weights. |
| Tue | - Convert the PyTorch model into ONNX format and apply dynamic quantization. <br> - Re-evaluate accuracy drop-offs versus speed gains (usually ~2x faster). |
| Wed | - Study Amazon CloudWatch components (Logs, Metrics, Dashboards, Alarms). |
| Thu | - Instrument the FastAPI code with CloudWatch Logs integration (using Boto3 CloudWatch client) to record endpoint latency per request. |
| Fri | - **Practice:** <br>&emsp; + Create a visual CloudWatch Dashboard monitoring ECS auto-scaling triggers, SQS backlog size, and average API latency <br>&emsp; + Set an Alarm to trigger when latency exceeds 5 seconds. |

### Week 10 Achievements:

- Successfully halved inference latency through Model Quantization and ONNX runtime optimization.
- Established comprehensive enterprise monitoring capabilities using CloudWatch.
- Converted implicit software delays into explicit, trackable metrics.

