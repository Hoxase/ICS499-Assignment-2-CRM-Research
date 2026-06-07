# ICS499-Assignment-2-CRM-Research
ICS499-Assignment 2 CRM research

# Exploring CRM Systems Using Generative AI

## Student Information

| Field        | Detail                                      |
|--------------|---------------------------------------------|
| Name         | O'Shae Berteaux                             |
| Course       | ICS499 – Software Engineering & Capstone    |
| Assignment   | Assignment 2 + FP1 (50 Points)              |
| Topic        | CRM Systems via Generative AI Research      |

---

# Deliverables

```text
exploring_crm_systems/

├── README.md
├── CRM_research_parts_1-4.md
├── prompts_used.md
├── references.md
├── architecture/
│   └── crm_architecture.png
└── screenshots/
    ├── login.png
    ├── dashboard.png
    ├── contacts.png
    ├── leads.png
    └── reports.png
```
---

## Executive Summary

This project documents an AI-assisted investigation of Customer Relationship Management (CRM) systems. Acting as a SW consultant, I used Claude (Anthropic), ChatGPT (OpenAI), and Perplexity AI to research the CRM landscape — from common concepts and commercial products to open-source solutions and custom architecture design.

Key findings:

## AI Tools Used
| Tool        | Provider   | Primary Use                                      |
|-------------|------------|--------------------------------------------------|
| Claude      | Anthropic  | Architecture design, writing, structured analysis |
| ChatGPT     | OpenAI     | Product comparisons, history research            |
| Perplexity  | Perplexity | Real-time pricing verification, source citations |

## CRM Research Findings
**Summary:** CRM (Customer Relationship Management) systems are software platforms that help organizations manage interactions with current and potential customers. They centralize contact data, automate workflows, track sales pipelines, and generate analytics

## CRM Product Comparisons
See full comparison tables in [`crm_research.md`](crm_research.md) — Part 2.

**Commercial CRM Highlights:**
- Salesforce: most powerful, most expensive
- HubSpot: best free-to-paid growth path
- Zoho CRM: best value for SMBs
- Microsoft Dynamics 365: best for Microsoft-ecosystem organizations

**Open-Source CRM Highlights:**
- SuiteCRM: most feature-complete, Salesforce-inspired
- EspoCRM: cleanest codebase, easiest to extend
- Odoo CRM: best if also needing ERP modules

## Open Source CRM Evaluation
**Selected:** Odoo 17 Community Edition (odoo.com/trial web instance)

Odoo's web-based trial environment was available immediately with no installation required. The CRM module presented a clean pipeline view by default, with leads and opportunities organized by stage. Navigation between modules, CRM, Contacts, and the activity log was intuitive, though the sheer number of available modules in the top menu took some orientation. The standout experience was how naturally the CRM connected to adjacent modules. The main limitation encountered in the Community tier was the absence of several features that appear prominently in the UI but are locked behind Enterprise


## CRM Architecture Proposal
**Stack:** HTML + CSS + Bootstrap + jQuery (front-end) | PHP (server-side) | MySQL (database)

The proposed architecture follows a classic MVC-inspired layered design:
- Browser renders Bootstrap-based views
- PHP handles routing, business logic, and authentication
- MySQL stores all relational CRM data

See the architecture diagram: [`architecture/crm_architecture.png`](architecture/crm_architecture.png)

Full module and database design details are in [`crm_research.md`](CRM_research_parts_1-4.md) — Part 4.

## Prompt Engineering Examples
See prompts_used.md for the five most effective prompts used during this project, along with analysis of AI strengths and weaknesses.

## Lessons Learned
1. **AI accelerates domain onboarding dramatically**
2. **Pricing data must always be verified**
3. **Prompt framing matters enormously**
4. **AI is excellent at architecture brainstorming** 


## References
See [`references.md`](references.md) for full citations.
