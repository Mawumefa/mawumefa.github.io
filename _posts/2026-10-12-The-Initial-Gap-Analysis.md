---
title: "The Initial Gap Analysis"
description: "How to run an initial ISO 27001 gap analysis: what it is, why it comes before the business case, and how to do it step by step, with interview questions for Clauses 4 to 10 and Annex A."
date: 2026-10-12 10:00:00 -0400
categories: [ISO27001]
tags: [iso27001, isms, grc, information-security, gap-analysis]
math: true
mermaid: true
comments: true
image:
   path: /commons/initial-gap-analysis-cover.jpg
   alt: Two cliffs labelled Today and Certified, with a measuring tape stretched across the gap and the question How far is it?
---

## The Initial Gap Analysis

*How to run an initial ISO 27001 gap analysis before the project starts.*

Welcome back! In the [last post]({{ '/posts/The-Full-ISO-27001-Roadmap/' | relative_url }}), we mapped the full journey from initiation to certification. Before MK Consults starts on any of it, we need to answer one question: where do we actually stand against the standard today?

A rough feel isn't enough. Management will be asked for budget, people and a year of commitment, and their first question will be how far we are from certification. The answer has to rest on evidence.

That's the job of the initial gap analysis. In this post I'll explain what it is, why you run it before the project starts, and how to do it step by step.

## What the initial gap analysis is, and why you run it

A gap analysis compares where an organization **is today** with where it **needs to be**, and records the difference: the gaps. The initial gap analysis is the first of two you run; the second is the detailed gap assessment, once the scope is approved. It is done **before the business case**, before any project exists, to answer management's first question with evidence: **how far are we from certification, and what will it take to get there?**

Who does it varies in practice. If the ISMS champion knows the standard well, they often run it themselves. Many organizations, though, bring in an external consultant for this first pass, because nobody in-house knows the standard well enough yet. In that case, management often approves a small budget for the gap analysis itself before the full business case. MK Consults is a security consultancy, so its CISO runs it in-house as ISMS champion.

It measures you against the requirements of ISO/IEC 27001:2022:

- **Clauses 4 to 10:** the mandatory management system requirements. Is there a policy? A risk process? Internal audit? Management review? Document control? Every one applies, so this is where most of the early work sits.
- **A quick pass through all 93 Annex A controls:** recording which controls already exist, based mainly on interviews, with lighter evidence checks than later on.

For each requirement it answers one question: is this in place, partly in place, or not in place? The findings let the ISMS champion:

1. **Describe the current state honestly.** The business case's Current State section rests on findings, not opinion.
2. **Size the work.** How much of the management system has to be built from scratch, and how much control work is likely.
3. **Estimate cost, people and time.** The external support needed, the internal time required and a realistic certification window, for the business case's Resources, Cost Overview and Timeline sections.
4. **Surface show-stoppers early,** before management commits money. For example, a client contract that requires certification by a date the gaps make impossible.
5. **Set a starting baseline,** so progress can be shown later.

I have created two templates for MK Consults for your reference to help guide your own work.

**MK Consults Initial Gap Analysis Workbook:** It lists every requirement of Clauses 4 to 10 and all 93 Annex A controls, with the documents needed and the evidence to confirm compliance, a drop-down to record whether each requirement is met, and a summary sheet that totals your results by clause and by Annex A section. Use it at a high level now, and in full for the detailed gap assessment later.

<iframe src="{{ '/assets/docs/MK-Consults_Initial_Gap_Analysis_Workbook.pdf' | relative_url }}?v=1#navpanes=0&view=FitH" width="100%" height="520" style="border: 1px solid #ccc; border-radius: 6px;" title="MK Consults Initial Gap Analysis Workbook" id="doc-gap-workbook"></iframe>

**Download:** [Excel (.xlsx)]({{ '/assets/docs/MK-Consults_Initial_Gap_Analysis_Workbook.xlsx' | relative_url }}?v=1) \| [PDF]({{ '/assets/docs/MK-Consults_Initial_Gap_Analysis_Workbook.pdf' | relative_url }}?v=1)

**MK Consults Initial Gap Analysis Readiness Summary:** The full report for MK Consults: executive summary, method, results by clause and Annex A section, key gaps, estimated effort, recommendations, and every clause and control rating in the appendices. Use it as a template for your own.

<iframe src="{{ '/assets/docs/MK-Consults_Initial_Gap_Analysis_Readiness_Summary.pdf' | relative_url }}?v=1#navpanes=0&view=FitH" width="100%" height="520" style="border: 1px solid #ccc; border-radius: 6px;" title="MK Consults Initial Gap Analysis Readiness Summary" id="doc-gap-readiness-summary"></iframe>

**Download:** [Word (.docx)]({{ '/assets/docs/MK-Consults_Initial_Gap_Analysis_Readiness_Summary.docx' | relative_url }}?v=1) \| [PDF]({{ '/assets/docs/MK-Consults_Initial_Gap_Analysis_Readiness_Summary.pdf' | relative_url }}?v=1)

## How you gather the evidence

Three techniques, used together:

- **Interviews:** ask people how things actually work.
- **Document review:** ask them to show you.
- **Light observation:** watch it happen, for example a screen-share of the user admin console.

The rule that makes or breaks the exercise: **evidence beats assertion.** "We do access reviews" is worth nothing until someone shows you the last one.

## Step 1: Prepare (days 1 to 2)

**Set your working scope** and write it down at the top of your notes. There's no formal ISMS scope yet, so use the same working assumption as the business case. At MK Consults: all staff, AWS, Microsoft 365, GitHub, the SaaS stack and the remote workforce.

**Set up your checklist.** Use the gap analysis workbook (download above). It lists every requirement of Clauses 4 to 10 and all 93 Annex A controls, with the documents and evidence to look for.

**Agree the rating scale** before you start, so you rate consistently:

| Rating | Meaning |
|---|---|
| Yes | Documented, operating, and you have seen the evidence |
| Partially | Done but not documented, documented but not done, or inconsistent |
| No | Not in place |
| Not applicable | Annex A only, and only where a control is clearly irrelevant, with a written reason. Treat it as provisional; the final decision is made in the Statement of Applicability |

In the initial analysis, note where a rating rests on interview only, so the detailed assessment knows what to evidence. Some practitioners prefer a 0 to 5 maturity scale instead. That works too, as long as it is simple enough to apply consistently in an interview.

**Send a document request list** a few days before the interviews, so people can gather things in advance. For example:

- any security policies, however old
- a list of systems or assets
- user access lists for key systems
- onboarding and offboarding checklists
- supplier contracts with security terms
- incident records
- backup reports
- the org chart and role descriptions

**Book the interviews.** Talk to the people who own each area, not just IT.

| Interviewee | Time | Main focus |
|---|---|---|
| CEO | 30 min | Clauses 4 and 5, risk appetite, objectives, management review |
| Head of IT | 90 min | Document control, operations, most technological controls |
| HR Manager | 45 min | Competence, awareness, people controls |
| Finance Manager | 30 min | Suppliers, asset purchasing, budget |
| Senior Consultant (client delivery) | 45 min | How client data is actually handled in delivery |
| External Legal and Compliance Advisor | 30 min | Legal, regulatory and contractual requirements, including GDPR |

A word on bias. At MK Consults the CISO runs the gap analysis as ISMS champion, which means security is partly self-assessed. That is normal in a small company, but be honest about it and hold your own area to a higher evidence bar than everyone else's.

## Step 2: Run the interviews (days 3 to 6)

**How to ask:**

- **Ask open questions.** "How do you give a new joiner access to AWS?" gets you a process. "Do you have an access process?" gets you a yes.
- **Follow every answer with "show me".** Then record what you saw.
- **Ask about the last time.** "When did someone last leave? Walk me through what happened to their accounts." Real events expose real practice.
- **Don't lead and don't judge.** You want the truth, not the answer people think you want.
- **Triangulate.** If IT says leavers lose access the same day, ask HR for the last leaver's date and compare it with when the account was disabled.
- **Take notes as you go:** the question, the answer, the evidence seen, the rating, and any follow-up.

## Step 3: What to ask, clause by clause

**Clause 4: Context of the organization**
- What internal and external issues affect our information security?
- Who expects us to protect information, and what exactly do they require: clients, regulators, insurers?
- Which laws and regulations apply to the information we handle, for example GDPR for client and employee personal data?
- Is climate change a relevant issue for us, and do any interested parties have climate-related requirements?
- Has anyone defined what the security program covers?
- Do we have anything like a management system for security today: defined processes, owners, and a way they fit together?
- *Ask to see:* client contracts and security questionnaires, any written scope.

**Clause 5: Leadership**
- Who at the top is accountable for information security?
- Is there an information security policy? Who approved it, and when?
- Are security roles defined and communicated? Who owns each system, and who approves access?
- *Ask to see:* the signed policy, role descriptions, any RACI.

**Clause 6: Planning**
- How do we identify and assess security risks today?
- Who decides what level of risk is acceptable?
- Do we have measurable security objectives?
- When we change how security is managed, how is that change planned and controlled?
- *Ask to see:* any risk register, risk criteria, targets or KPIs.

**Clause 7: Support**
- Who has security skills, and how do we know they are competent?
- Does everyone get security awareness training? When was the last session?
- Who communicates what about security, to whom, and when?
- How are documents controlled: versions, approval, storage?
- *Ask to see:* training records, certifications, a sample document's version history.

**Clause 8: Operation**
- How are security activities planned and controlled day to day?
- Has a risk assessment ever been carried out and acted on?
- How do we control what we outsource, for example AWS and our SaaS tools?
- *Ask to see:* tickets, schedules, supplier reviews.

**Clause 9: Performance evaluation**
- What do we measure about security, and who looks at it?
- Has anyone ever audited our security practices internally?
- Does management formally review security?
- *Ask to see:* reports, audit reports, minutes.

**Clause 10: Improvement**
- When something goes wrong, how is it recorded and fixed?
- Do we look for root causes, or just fix the symptom?
- *Ask to see:* an incident or issue log and a sample record.

## Step 4: Make a quick pass through Annex A

Walk through all 93 controls in order and give each one a headline status. Ask the control owner how it is done, and check evidence where it is quick to see, such as the MFA settings or the asset list. Many controls go quickly in a small company because the answer is obvious. Some example questions for each Annex A section:

- **A.5 Organizational controls:** Is there an asset inventory? How is access granted, reviewed and removed? How are suppliers assessed? How are incidents handled? Is there a continuity plan? How is personal data identified and protected?
- **A.6 People controls:** Are new joiners screened? Do they sign confidentiality terms? What happens on the day someone leaves? Are there rules for remote working?
- **A.7 Physical controls:** How are laptops protected when people work from home? What happens to equipment and paper at the office?
- **A.8 Technological controls:** Is MFA enforced everywhere? Are endpoints managed and encrypted? Are backups tested? Are logs collected and reviewed? How are vulnerabilities found and patched? How is code reviewed before it goes live?

Record what is in place. Leave the decision on what applies for later.

## Step 5: Analyze (days 7 to 8)

- **Rate every clause requirement and every Annex A control,** noting the evidence behind each rating.
- **Separate the two kinds of gap:** missing management system processes (Clauses 4 to 10) and control areas where current practice is weak.
- **Estimate the effort.** For each major gap, decide whether it means writing something (a policy, a procedure), building something (a risk process, an internal audit program) or implementing something (a technical control).
- **Translate it into the business case:** the people you need, the external help you will buy, a realistic timeline and the budget.

## Step 6: Write the readiness summary (days 9 to 10)

Keep the main body short, a few pages that management will actually read, and put the full clause and control ratings in appendices for anyone who wants the detail.

1. **Purpose, working scope, method and who you interviewed.**
2. **A clause-by-clause heat map** for Clauses 4 to 10: each clause color-coded green, amber or red by its rating.
3. **An Annex A summary by section (A.5 to A.8):** how many controls are in place, partly in place or not in place.
4. **The top five to eight gaps,** one line each, with the evidence behind them.
5. **Implications:** estimated effort, external support needed and a realistic certification window.

This summary is what feeds the Current State, Resources, Cost Overview and Timeline sections of the business case.

## What's next

With the readiness summary in hand, the ISMS champion has the evidence to make the case. In the next post, we draft the business case and present it to management.

Thanks for reading, see you in the next post.

**Mawumefa**  
*Your Audit Ally*

*MK Consults is a fictitious company. All names, figures and documents in this series are illustrative and created for educational purposes.*

{% include documents-so-far.html %}

## Sources

- [ISO/IEC 27001:2022, Information security management systems: Requirements](https://www.iso.org/standard/27001)
- [ISO/IEC 27001:2022/Amd 1:2024, Climate action changes](https://www.iso.org/standard/88435.html)
- [ISO/IEC 27002:2022, Information security controls](https://www.iso.org/standard/75652.html)
- [ISO/IEC 27007:2020, Guidelines for information security management systems auditing](https://www.iso.org/standard/77802.html)
