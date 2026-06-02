# Assignment Overview

Modern software professionals increasingly use Artificial Intelligence (AI) tools such as ChatGPT, Claude, Gemini, Perplexity, and GitHub Copilot to accelerate learning, research, software evaluation, solution design, and documentation.

In this assignment, you will use AI as your research assistant to explore the world of Customer Relationship Management (CRM) systems.

The purpose of this assignment is not to become a CRM expert. Instead, the goal is to demonstrate your ability to:

* Learn a new software domain using AI
* Ask effective questions
* Compare competing software products
* Explore open-source solutions
* Analyze software architecture
* Critically evaluate AI-generated content
* Produce professional technical documentation

Think of yourself as a software consultant who has been assigned to investigate CRM systems and provide recommendations to a company considering CRM adoption.

---

# Learning Objectives

By completing this assignment, you should be able to:

* Explain what CRM systems are and why organizations use them.
* Use Generative AI tools effectively for technical research.
* Compare commercial and open-source CRM products.
* Install and evaluate an open-source CRM solution.
* Understand the architecture of a CRM application.
* Reflect on the strengths and limitations of AI-assisted research.
* Create a professional technical report using Markdown.

---

# AI Usage Requirements

This is an AI-assisted assignment.

You are encouraged to use one or more of these AI tools.

* ChatGPT
* Claude
* Gemini
* Perplexity
* GitHub Copilot
* Microsoft Copilot


You must document:

* Which AI tools you used
* Sample prompts you entered
* How AI helped your research
* Any incorrect or incomplete AI-generated responses
* How you validated information


---

# Part 1 (COMPLETE) – AI-Based CRM Discovery (10 Points)

Use one or more AI tools to research CRM systems.

### Q1. What is CRM?

* Definition
  * A CRM (customer Relationship managment) is a software meant to manage a company's relationship and interaction with its exisiting a potential customers as well as a place to centralize customer data, automate workflows, and provide analytics to help nuture relationships and grow revenue 
* Purpose
  * The core purpose of a CRM system is to improve business relationships. Specifically:
    - Centralize customer and prospect data in a single, accessible location
    - Track calls, emails, meetings, purchases across the customer lifecycle
    - Enable sales, marketing, and support to collaborate efficently 
    - Automate repetitive tasks like follow-up emails, lead scoring, and pipeline stage updates
    - Provide visibility into sales performance and customer health
* History
  * 2000s: Salesforce launched in 1999 and popularized the Software-as-a-Service (SaaS) delivery model, eliminating on-premise installation. 
  * 2010s: CRM expanded into marketing automation, customer support, and social media integration. Mobile CRM became standard.
  * 2020s: AI and machine learning are embedded into CRM platforms for predictive lead scoring, conversation intelligence, churn prediction, and generative content suggestions.
* Evolution
  * CRM has evolved from a simple  rolodex -> full sales force automation -> cloud SaaS -> AI-driven relationship intelligence.
---

### Q2. Why do organizations use CRM systems?


* Sales management
  * CRM's provide a structrured view of every deal in rpogress
* Customer management
  * All customer data and info is consolidated to one place (contact info, communication history, purchase records, preferences, and support tickets)
* Marketing
  * CRM systems power targeted marketing by segmenting customers based on behavior, purchase history, or demographic data.
* Customer support
  * Most CRM inlcude a ticketing system where agents can manage, escelate, track, and solve issues
* Reporting and analytics
  * Dashboards and reports give visibility into KPIs such as average deal size, customer acquisition cost, customer lifetime value, churn rate, and support ticket volume. These insights drive strategic decisions

---

### Q3. What business problems do CRM systems solve?

Provide examples from:

* Retail
  * Resolves customer data scattered across multiple systems eg point-of-sale systems, loyalty programs, and email lists by centralizing it all in one place  
* Healthcare
  * They automate appointment reminders, track theyre health care jpurmey, and ensure HIPAA compliance
* Education
  *Track students enrollment and progress throguhtout their journey in school
* Manufacturing
  * Track vendors, spending, quotes,
* Nonprofits
  * Track donation hisory and engagment

---

### Q4. What are the major modules found in a CRM?

* Contacts: Store individual person records (name, email, phone, company, history)
* Accounts: Store organization records and can link multiple contacts to one account
* Leads: Track unqualified prospects
* Tasks: Assign and track to-do items for users 
* Customer Support Tickets: Log customer issues; track resolution status.
* Reports: Pre-built and custom data queries and exports  
* Dashboards: Visual KPI (Key Performance Indicator) displays; real-time metrics for management 

---

## Reflection

For each major topic, answer:

* Which AI tool generated the response?
  * Claude
* Was the response complete?
  * Complete
* Did you verify the information?
  * Yes, I cross-referenced against documentation and online summerizations.
* How trustworthy was the result?
  * High. Module definitions are well-established in the industry.    


---

# Part 2 (COMPLETE) – AI-Assisted CRM Product Comparison (10 Points)

Use AI to research and compare CRM products.

## Commercial CRM Products

Research at least four commercial CRM systems.

Suggested products:

* Salesforce
* HubSpot CRM
* Zoho CRM
* Microsoft Dynamics 365 CRM
* Oracle CRM

Create a comparison table.

| Product | Target Customer | Strengths | Weaknesses | Pricing Model |
| ------- | --------------- | --------- | ---------- | ------------- |
| **Salesforce**              | Mid-market to Enterprise     | Most feature-rich platform; massive ecosystem; AI (Einstein); AppExchange marketplace | Expensive; complex setup; steep learning curve      | Per user/month; starts ~$25; enterprise plans $300+ |
| **Zoho CRM**                | SMB to Mid-market            | Affordable; comprehensive feature set; strong automation; good API | UI feels dated; support quality varies; large product family can be confusing | Per user/month; starts ~$14; free for up to 3 users |
| **Microsoft Dynamics 365**  | Enterprise | Deep Office 365/Teams integration; Power Platform extensibility; strong ERP connection | High cost; complex licensing; requires IT expertise  | Per user/month; starts ~$65 (Sales Professional) |
| **Oracle CX (CRM)**         | Large Enterprise             | Enterprise-grade scalability; strong analytics; global compliance | Very expensive; heavy implementation burden; overkill for most | Custom enterprise pricing               |

---

## Open Source CRM Products

Research at least three open-source CRM systems.

Suggested products:

* SuiteCRM
* EspoCRM
* Odoo CRM
* Vtiger CRM

Create a comparison table.

| Product | Features | Technology Stack | Community Support | Ease of Installation |
| ------- | -------- | ---------------- | ----------------- | -------------------- |
| **SuiteCRM**   | Full sales, marketing, support; Salesforce-comparable modules; detailed reporting | PHP, MySQL, Bootstrap             | Large; active forums; commercial support available | Moderate — requires LAMP stack; Docker option available |
| **Odoo CRM**   | CRM module + optional ERP modules (inventory, accounting, HR)             | Python (Odoo framework), PostgreSQL | Very large; enterprise support | Moderate — Docker; Odoo.sh cloud option |
| **Vtiger CRM** | Sales, support, marketing in one; AI scoring features; inventory          | PHP, MySQL                        | Medium; commercial Vtiger One SaaS option | Moderate — traditional installer; some Docker support |

---

## Analysis

Discuss:

* Which commercial CRM appears most popular?
  * with at least 21% of the global CRM market, salesforce is by far the most popular
* Which open-source CRM appears most mature?
  * SuiteCRM as it has been in  development for over a decade and is a fork of another mature and extensive opensource CRM    
* Which CRM would you recommend for a small business?
  * Hubsport as it has a free tier which inlcuded unlimited users and required no IT support to deploy as well as can easily scale with the company
* Which CRM would you recommend for a large enterprise?
  * Salesforce as it has an indepth ecosystem with a wide range of customization capapbilities as well as compliance certififcations

---

# Part 3 (COMPLETE) – Open Source CRM Exploration (10 Points)

Select ONE open-source CRM and explore it ( SuiteCRM, EspoCRM, Odoo CRM, Vtiger CRM )

I went with Odoo

---

## Required Screenshots

Capture and include screenshots of:

* Login Screen
 * <img width="1749" height="606" alt="image" src="https://github.com/user-attachments/assets/79fba89c-961f-466b-bfa2-475b3796dce4" />
* Dashboard
 * <img width="1708" height="782" alt="image" src="https://github.com/user-attachments/assets/dfb598dc-f261-43cf-9e73-fb6a60aaad96" />
* Contacts Module
 * <img width="1706" height="464" alt="image" src="https://github.com/user-attachments/assets/ebe0abc8-6b5e-4143-a7d9-0ded8a28b87e" />
* Leads Module
 * <img width="1704" height="986" alt="image" src="https://github.com/user-attachments/assets/3919313f-2c32-40db-a58d-200e0416b196" />
* Reports or Analytics Module
 * <img width="1703" height="659" alt="image" src="https://github.com/user-attachments/assets/42f50535-1e37-47cb-98d5-31fd4cabbb48" />
 

---

## Evaluation Questions

Answer the following:

### Installation Experience

* Was installation easy?
  * Yes it's web based so i didnt need to install anything just created a account
* What challenges occurred?
  * none so far it's pretty intuitive
* How did AI help?
  * suggetsed i as a easy lightweight solution

### Product Experience

* What features impressed you?
  * Nothin in paticular, most features seems standard with most CRM's
* What features were missing?
  * None that I can think of or rather I have nothing to compare ti to aside from Jira and DevOps, at most PaaS and IaaS integration like with DevOps
* Would you use it in a real organization?
  * Yes I would

Explain your reasoning.

---

# Part 4 (INCOMPLETE) – AI-Assisted CRM Architecture Exploration (10 Points)

Assume your organization wants to build a CRM system using the following technology stack:

### Front-End

* HTML
* CSS
* JavaScript
* jQuery
* Bootstrap

### Server-Side

* PHP

### Database

* MySQL

Use AI tools to investigate how such a CRM might be designed.

---

## Questions

### Functional Modules

What modules should be included?

Examples:

* Authentication
* Contacts
* Leads
* Opportunities
* Tasks
* Reports

---

### Database Design

What tables would be required?

Examples:

* Users
* Roles
* Contacts
* Leads
* Accounts
* Opportunities
* Activities
* Tickets

---

### Useful Libraries

Research libraries that could accelerate development.

Examples:

* Bootstrap
* DataTables
* Chart.js
* PHPMailer
* Composer

Explain the purpose of each library.

---

### Security Considerations

Research:

* Authentication
* Authorization
* Password Security
* SQL Injection Prevention
* Cross-Site Scripting (XSS)
* Data Privacy

---

### MVP Proposal

Describe the smallest useful CRM that could be built.

What features would be included in Version 1?

---

## Architecture Diagram

Create a simple architecture diagram showing:

```text
Browser
   |
HTML/CSS/JS/Bootstrap
   |
PHP Application Layer
   |
MySQL Database
```

You may use of of these tools:
* Excalidraw
* Draw.io
* Mermaid

Include the diagram in your report.

---
