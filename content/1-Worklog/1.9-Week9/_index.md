---
title: "Week 9 Worklog"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:
- Research and integrate Large Language Models (LLM) as a fallback mechanism.
- Utilize Google Gemini / Amazon Bedrock for processing severely unstructured documents.
- Design multi-modal prompt engineering flows.

### Tasks for the Week:

| Day | Tasks |
| --- | --- |
| Mon | - Analyze edge cases that the traditional LayoutLM completely fails to read (Handwritten bills, faded dot-matrix prints). |
| Tue | - Research LLM capabilities for multimodal extraction. <br> - Obtain Gemini API keys / configure AWS Bedrock models (Anthropic Claude). |
| Wed | - Design specialized Prompt Engineering templates. instructed the LLM to output stricly JSON formats replicating the local schema. |
| Thu | - Implement the Fallback Pipeline: If local model confidence < 80%, send Image payload to LLM endpoint directly and parse JSON. |
| Fri | - **Practice:** <br>&emsp; + Feed 50 extreme-case invoices to the Gemini/Bedrock pipeline <br>&emsp; + Measure hallucination rates and adjust the system prompts accordingly. |

### Week 9 Achievements:

- Successfully integrated leading generative AI solutions to drastically reduce absolute failure rates.
- Gained advanced Prompt Engineering skills ensuring schema conformity from LLMs.
- Built a dual-tier OCR architecture combining cost-effective local AI and powerful cloud LLMs.

