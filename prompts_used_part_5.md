# Part 5 – AI Reflection and Prompt Engineering (10 Points)

This file documents the most effective prompts used during this CRM research project, along with analysis of AI performance.

---

## Best Prompts

### Prompt 1 – CRM Domain Introduction

**Tool Used:** Perplexity

**Prompt:**
```
Act as a senior software consultant explaining CRM systems to a computer science student 
who has strong programming skills but no business software background.

Explain:
1. What CRM systems are (definition and purpose)
2. The history of CRM software
3. Why organizations invest in CRM systems

Use concrete examples. Avoid marketing language and be technically honest
```

**Why I think It Worked:**
- I beilive the specification ("strong programming skills, no business background") calibrated the technical depth correctly.
- Explicitly asking to "avoid marketing language" and "be technically honest" produced a more balanced response than a plain question would have.
- Numbered structure in the prompt produced a structured, organized response.

**Result Quality:** Excellent. The response clearly separated genuine CRM value which I would not have gotten from a generic "What is CRM?" query.


---

### Prompt 2 – Open Source CRM Evaluation

**Tool Used:** ChatGPT

**Prompt:**
```
I am evaluating open-source CRM systems for a small nonprofit . 
We need: contact management, donation tracking, volunteer management, and basic reporting.
We have one part-time IT person who can manage a Linux server.

Compare SuiteCRM, EspoCRM, and Odoo CRM for this specific use case.

For each:
- List which of our required features are available out-of-the-box vs. requiring extensions
- Identify any hidden complexity
- Give a final recommendation with reasoning

Be honest about limitations.
```

**Why I think It Worked:**
- The specific use case made the comparison contextual rather than generic.
- Listing specific requirements meant the AI addressed each one rather than giving a generic feature overview.
- "Be honest about limitations consistently produces more candid AI responses.

**Result Quality:** Excellent. The response correctly identified that Odoo requires more technical overhead than EspoCRM and that SuiteCRM's donation tracking is more mature — both accurate points that other sources confirmed.

---

### Prompt 3 – Database Schema Design

**Tool Used:** Claude

**Prompt:**
```
I am designing a CRM system using PHP and MySQL. 

Design a normalized MySQL database schema for a CRM with these modules:
- Users with role-based access control
- Contacts (individual people)
- Accounts (companies)
- Leads (unqualified prospects)
- Opportunities (active deals)
- Activities (calls, meetings, notes)
- Tasks

Requirements:
- Support soft deletes (preserve data for audit purposes)
- Every entity should have an assigned user (for ownership filtering)
- Activities and Tasks should be able to link to any entity type

Show:
1. CREATE TABLE statements for each table
2. Explain any design decisions that aren't obvious
3. Point out any normalization tradeoffs I should consider
```

**Why I think It Worked:**
- Providing the specific requirements (soft deletes, polymorphic relationships) meant the schema addressed real design constraints.
- Asking for "design decisions that aren't obvious" surfaced non-obvious choices like the polymorphic `related_type`/`related_id` pattern.


**Result Quality:** Very good. The generated schema was production-quality with appropriate foreign keys, soft delete columns, and indexing recommendations. I modified the naming conventions to match my preferences.

---

### Prompt 4 – Security Review

**Tool Used:** Claude

**Prompt:**
```
I am building a PHP/MySQL web application (a CRM system) and need a security review checklist.

The application will:
- Handle login/authentication
- Store personally identifiable information (names, emails, phone numbers)
- Be accessible over the public internet

Cover these security areas:
1. Authentication (session management, password storage)
2. SQL injection prevention
3. Cross-site scripting (XSS)
4. CSRF protection
5. Data privacy / compliance basics (GDPR awareness)

For each area:
- Explain the threat
- Give the PHP-specific mitigation
- Show a code example where relevant
- Rate the implementation complexity (easy / moderate / complex)

Be specific to the most commonly used PHP version and PDO. Do not give generic web security advice.
```

**Why I think It Worked:**
- Specifying "most commonly used PHP version" prevented generic security advice that wasn't applicable to the stack.
- The scenario context (public internet, PII data) appropriately scoped the severity of the recommendations.

**Result Quality:** Excellent. The PHP-specific code examples (PDO prepared statements, `password_hash()`, CSRF token generation) were usable and the GDPR section was high-level.

---

## AI Effectiveness Analysis

### What AI Did Well

**Structured comparisons:** When given clear dimensions (target customer, strengths, weaknesses, pricing), the AI produced clean comparison tables that would have taken hours to assemble from individual vendor websites.

**Architecture brainstorming:** AI is exceptionally useful for "what should I consider" questions. The database schema, module list, and security checklist were all high-quality starting points that only needed refinement, not rewriting.

**Explaining unfamiliar domains:** Starting with only some  CRM knowledge, AI helped further explained the domain in a calibrated, technically grounded way within minutes. whihc is a clear advantage over traditional research.

**Code generation:** The PHP/MySQL examples 

---

### What AI Struggled With

**Current pricing:** Pricing for Salesforce, HubSpot, and Zoho can change frequently. AI responses contained pricing that was somehwat accurate but required Perplexity or my own research to verify current pricing.

**Nuanced tradeoffs:** AI tends to hedge recommendations ( example: "it depends on your specific needs") rather than committing. Prompts that force a recommendation produced more useful outputs.

**Hallucinations**: while AI is tranformative in work flows, leanring, boirlerplate, and research it can tend to hallicinate as in give you incorrect adn soemtime non existent answers and info just to give you the answer you want despite having the info that contradicts said claims

---

### What Information Required Validation

- All pricing figures (verified on vendor websites)
- EspoCRM Docker Compose configuration (verified against official GitHub repository)
- HIPAA CRM compliance claims (verified against HHS.gov)
- Library version compatibility (Bootstrap 5 vs. 4 DataTables compatibility — AI gave outdated info; checked npm documentation)

---

### What Surprised Me

The quality of AI-generated database schemas was unexpectedly high. I expected non-normalized schema that I would need to rework. Instead, the schema included appropriate use of soft deletes, polymorphic relationship patterns, and indexing recommendations that reflect genuine database designs.

Also surprising: explicitly telling the AI to "be honest about limitations" and "don't recommend something you cant easily defend or explain in a high level" consistently changed the tone of responses from promotional to candid. This framing should be standard practice.

---

### What I Would Do Differently Next Time

1. Start with Perplexity for pricing and product facts for its live search prevents the outdated-pricing problem.
2. Use Claude for architecture and design for its reasoning on system design questions is consistently strong.

3. Ask for a "devil's advocate" response as to argue agaisnt it to see multipel point of views**

4. Specify output format explicitly as this saves on thinking and generation time

5. Iterate the prompt before accepting the response meaning always follow up on the first response with refinements and clarifications as toimprove quality for the first response is rarely the best; .

---

### Would You Trust AI for Software Research?

**Yes but usually as a starting point, not an ending point.**

AI dramatically accelerates the initial learning curve for unfamiliar topics. In this project, it compressed what might have been two weeks of reading into several hours hours across a few days of targeted Q&A. For a software professional, this is genuinely useful.

However, AI has real failure modes that matter in professional contexts depending on the model used:
- **Outdated information**: pricing, library versions, and product features change; AI does not.
- **Confident incorrectness**: AI does not signal uncertainty when it should. Treat all specific claims as hypotheses to verify.
- **No hands-on experience**: AI can describe an installation process but cannot tell you it will fail on a specific OS version until you encounter the error yourself.


The right  model: **AI is like a well-read colleague who has read everything but done nothing.** Its breadth of knowledge is extraordinary; its operational experience is zero in whihc it is best used for orientation, structure, and first drafts. Use primary sources and hands-on testing for verification and production.

