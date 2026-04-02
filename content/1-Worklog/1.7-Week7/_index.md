---
title: "Week 7 Worklog"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:
- Tackle the complex line item (table) extraction problem.
- Store structured parsed JSON into a relational or NoSQL database.
- Use Amazon RDS / DynamoDB for persistent record storage.

### Tasks for the Week:

| Day | Tasks |
| --- | --- |
| Mon | - Analyze failure patterns in invoice table bounding boxes (merged columns, multiline items). <br> - Research graph modeling or YOLOV8 bounding logic for table detection. |
| Tue | - Write complex heuristics algorithms to group table cells logically by Y-coordinates (row clustering). |
| Wed | - Explore Amazon RDS (PostgreSQL) vs DynamoDB. <br> - Decide on PostgreSQL to easily map relationships between 'Invoices' and 'Line Items'. |
| Thu | - Set up an Amazon RDS PostgreSQL instance in a private Subnet. <br> - Connect securely using DBeaver or pgAdmin via Bastion Host/VPN. |
| Fri | - **Practice:** <br>&emsp; + Extend the FastAPI logic to insert OCR results directly into the RDS database via SQLAlchemy <br>&emsp; + Verify data insertions and schema integrity. |

### Week 7 Achievements:

- Engineered an advanced spatial heuristic logic to parse variable-format invoice tables effectively.
- Understood AWS networking isolation (Private Subnets, Bastion Hosts).
- Integrated persistent relational database storage (Amazon RDS) with the OCR API.

