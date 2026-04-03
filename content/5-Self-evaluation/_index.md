---
title: "Self-Assessment"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 6. </b> "
---

During my internship with the SmartInvoice Shield project from January 2026 to April 2026, I had the opportunity to learn and apply industry-leading AI models and AWS Cloud services to a real-world invoice management solution.
I was directly involved in researching, developing, and optimizing the core AI OCR pipeline, ensuring seamless integration with the system's Backend.

### Key Contributions & Technical Highlights

**1. Advanced AI Model Development & Integration**
- Directly participated in designing the multi-tier AI OCR architecture, heavily utilizing the **Gemini API** for robust and highly dynamic invoice data extraction.
- Trained and implemented **LayoutLMv3** for layout-aware document understanding, backing it up with a custom **PaddleOCR + VietOCR** pipeline to establish a high-accuracy, cost-effective baseline.
- Engineered a rigorous **Rule Engine** at the post-processing layer to validate extracted data (e.g., cross-checking subtotals and parsed units) ensuring strict schema integrity.

**2. Cloud Deployment (AWS) & Integration**
- Taking on the role of AI Engineer, I directly tuned the AI models for containerized deployment, ensuring a frictionless integration with the Backend (.NET 9) running on AWS ECS Fargate Spot.
- Worked closely with the Backend track to resolve asynchronous processing hurdles, ensuring the AI inference clusters could safely consume workloads queued on Amazon SQS.
- Effectively monitored and managed AI inference costs by strategically balancing calls between the paid Gemini API and the on-premise LayoutLMv3.

**3. System Optimization & Troubleshooting**
- Successfully optimized and integrated the combined AI OCR pipeline into the larger ecosystem.
- Resolved complex constraints regarding OCR latency and LLM Hallucinations by iteratively testing Prompt Engineering strategies.
- Proactively proposed and built the **AI Fallback logic**: routing straightforward invoices through the localized OCR stack and dispatching overly unstructured or badly scanned invoices to Gemini, drastically enhancing reliability.

### Self-Assessment

To objectively reflect on my internship period, I would like to evaluate myself based on the following criteria:

| No. | Criteria | Evaluation | Comments |
|---|---|---|---|
| 1 | Professional Knowledge | ✅ Good | Mastered the deployment of advanced CV/NLP models (LayoutLMv3, PaddleOCR, Gemini API) and AI wrapper integrations on AWS. |
| 2 | Learning Ability | ✅ Good | Rapidly acquired GenAI prompt techniques and conquered the hyperparameter tuning for layout-aware models treating complex Vietnamese templates. |
| 3 | Proactiveness | ✅ Good | Actively proposed the Tiered AI Fallback logic to maximize accuracy while minimizing API operational costs. |
| 4 | Discipline | ✅ Fair | Strictly adhered to the project schedule, synced seamlessly with backend deployments, and maintained detailed weekly worklogs. |
| 5 | Communication | ✅ Fair | Clearly communicated AI architecture logic to non-tech peers and rapidly resolved JSON payload contracts with Backend developers. |
| 6 | Teamwork | ✅ Good | Collaborated efficiently across Backend, Frontend, and Cloud tracks to ensure synchronized SmartInvoice Shield operations. |
| 7 | Problem Solving | ✅ Good | Effectively mitigated logic bottlenecks in OCR latency, tamed LLM hallucinations, and constructed a fail-safe Rule Engine. |
| 8 | Project Contribution | ✅ Good | Successfully delivered the high-precision core AI OCR engine, establishing the foundational intelligence of the entire project. |

### Needs Improvement
- Strengthen discipline in updating technical documentation and precision metrics immediately after every minor model configuration change.
- Improve presentation skills for visualizing complex machine learning training workflows to make them easier to digest for business stakeholders.
- Continue exploring advanced deep learning compilation (like ONNX runtime) to further optimize local inference speeds in the future.
