---
title: "Week 5 Worklog"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:
- Understand and train layout-aware transformers (LayoutLM/Donut).
- Leverage AWS GPU instances / SageMaker for accelerated training.
- Identify loss convergence and avoid overfitting.

### Tasks for the Week:

| Day | Tasks |
| --- | --- |
| Mon | - Research Layout-aware models (LayoutLMv3, Donut) capable of reading spatial data over images. <br> - Compare compute options: EC2 G-series vs Amazon SageMaker Notebooks. |
| Tue | - Provision a GPU-backed instance (e.g., g4dn.xlarge). <br> - Configure CUDA toolkits to utilize the NVIDIA GPUs for PyTorch. |
| Wed | - Prepare the augmented datasets from S3 into PyTorch Dataloaders format (tokenizing text & boxes). |
| Thu | - Fine-tune the LayoutLMv3 model for document token classification (Entity Extraction). <br> - Monitor training epochs and validation loss. |
| Fri | - **Practice:** <br>&emsp; + Save model checkpoints iteratively to S3 using multi-threading <br>&emsp; + Test the trained weights on a separate holdout dataset. |

### Week 5 Achievements:

- Deployed and configured GPU-accelerated computing infrastructure on AWS.
- Successfully fine-tuned a state-of-the-art transformer model on custom OCR data.
- Learned how to sync massive training weights seamlessly with cloud storage.

