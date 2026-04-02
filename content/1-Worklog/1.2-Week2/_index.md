---
title: "Week 2 Worklog"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Week 2 Objectives:
- Familiarize with AWS S3 for storing large invoice datasets.
- Evaluate baseline OCR models (Amazon Textract and Tesseract).
- Identify limitations in existing OCR tools for Vietnamese invoices.

### Tasks for the Week:

| Day | Tasks |
| --- | --- |
| Mon | - Provision Amazon S3 buckets for storing raw and processed invoice images. <br> - Set up IAM policies for restrictive S3 access. |
| Tue | - Research and set up Tesseract OCR locally (or on EC2) for baseline testing on Vietnamese invoices. |
| Wed | - Explore Amazon Textract API using Boto3 (AWS SDK for Python). <br> - Run sample invoices through Textract and extract raw text blocks. |
| Thu | - Compare Tesseract and Textract results. <br> - Document common failure cases (e.g., blurry text, complex tables, stamps overlapping context). |
| Fri | - **Practice:** <br>&emsp; + Upload 100 sample invoices to S3 <br>&emsp; + Write a Python script to fetch from S3, run Textract, and store raw JSON results locally. |

### Week 2 Achievements:

- Successfully configured Amazon S3 buckets with proper IAM permissions for programmatic access.
- Gained hands-on experience using Boto3 to interact with AWS services.
- Evaluated and understood the limitations of standard OCR models (Textract, Tesseract) with unstructured Vietnamese invoices.

