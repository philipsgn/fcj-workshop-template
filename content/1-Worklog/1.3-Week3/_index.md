---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:
- Understand serverless computing via AWS Lambda.
- Build an automated image pre-processing pipeline for invoices.
- Apply OpenCV for image quality improvements (deskew, binarization).

### Tasks for the Week:

| Day | Tasks |
| --- | --- |
| Mon | - Study AWS Lambda concepts and execution environments. <br> - Research S3 Event Notifications architecture. |
| Tue | - Research image processing techniques using OpenCV. <br> - Develop algorithms for image deskewing (straightening) and noise reduction. |
| Wed | - Develop binarization (thresholding) algorithms to enhance faded text on carbon copy invoices. <br> - Test processing scripts locally. |
| Thu | - Package the OpenCV Python script into a Lambda Layer to overcome size limitations. <br> - Deploy the data processing Lambda function. |
| Fri | - **Practice:** <br>&emsp; + Configure S3 Event trigger to invoke Lambda on object creation <br>&emsp; + Test the end-to-end pipeline: Upload image to input bucket -> Lambda processes -> Output to processed bucket. |

### Week 3 Achievements:

- Mastered AWS Lambda packaging, deploying Lambda Layers with third-party libraries (OpenCV).
- Successfully built an event-driven architecture using S3 triggers.
- Created a robust image preprocessing module improving downstream OCR accuracy.

