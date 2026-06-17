---
name: clinical-recommendation-extractor
description: >
  Transform clinical guidelines, research papers, implementation reports,
  and healthcare evidence into implementation-ready action plans,
  stakeholder maps, risk assessments, and execution roadmaps.
domain: healthcare
subdomain: clinical-implementation
tags:
  - healthcare
  - clinical-implementation
  - clinical-guidelines
  - evidence-synthesis
  - digital-health
  - medtech-deployment
version: "1.0.0"
author: Francis Okorie Iyeke-Kanu
license: Apache-2.0
---

# Clinical Recommendation Extractor

## When to Use

Use this skill when the user asks to:

- Analyze a clinical guideline
- Review a healthcare research paper
- Extract actionable recommendations
- Create an implementation roadmap
- Identify implementation barriers
- Translate evidence into operational plans
- Prepare implementation workshops
- Evaluate digital health adoption requirements

## When Not to Use

Do not use this skill when:

- The user only wants a simple summary
- The document is not healthcare-related
- Statistical analysis is the primary objective
- The user requests legal or regulatory advice

## Prerequisites

The user should provide one or more of:

- Clinical guideline
- Research paper
- Whitepaper
- Health technology assessment
- Product evaluation report
- Clinical implementation report

If critical information is missing, ask clarifying questions before proceeding.

## Context Intake (Mandatory Before Planning)

Before creating any implementation plan, collect institution-specific context.
If the user asks for a plan immediately, pause and ask targeted discovery
questions first.

Minimum context to collect:

- Facility profile (hospital type, size, inpatient/outpatient mix)
- Care setting and service lines affected (ED, ICU, ambulatory, etc.)
- Patient population and case complexity
- Current-state workflow and baseline performance
- Existing technology stack (EHR, integrations, medical devices, analytics)
- Staffing model and available implementation capacity
- Budget constraints and procurement limits
- Regulatory/compliance constraints and internal policy requirements
- Timeline constraints and executive priorities
- Implementation owner, governance structure, and decision rights

Use this question bank when details are missing:

1. What type of institution is this (academic medical center, community
   hospital, clinic network), and approximately how large is it?
2. Which departments and care settings will be in scope for this plan?
3. What is the primary patient population and any high-risk segments?
4. What does the current workflow look like today, and where are the biggest
   pain points?
5. Which systems must this plan integrate with (EHR, LIS, RIS, billing, etc.)?
6. What staffing capacity is available for implementation over the next 90 days?
7. What budget guardrails or procurement constraints should be assumed?
8. Are there regulatory, accreditation, or internal policy constraints we must
   satisfy?
9. Who are the executive sponsor and operational owner, and how are decisions
   approved?
10. What outcomes matter most in the first 30 days (safety, throughput, cost,
    adoption, patient experience)?

If the user cannot provide all answers:

- Continue with best-effort planning.
- Add an assumptions section to the output.
- Label each assumption with confidence (high/medium/low).
- Flag high-impact unknowns as blockers or validation checkpoints.

## Workflow

### Step 1: Institution Context Profile

Synthesize responses into a concise context profile that includes:

- Institution characteristics
- Scope boundaries
- Operational constraints
- Technology and data dependencies
- Governance and ownership model

### Step 2: Clinical Objective

Determine:

- Primary problem addressed
- Target population
- Intended outcomes

### Step 3: Recommendation Extraction

Identify:

- Explicit recommendations
- Implicit recommendations
- Best-practice guidance
- Required workflow changes

### Step 4: Stakeholder Identification

Identify all relevant stakeholders:

- Physicians
- Nurses
- Clinical leadership
- IT teams
- Biomedical engineering
- Operations
- Patients
- External vendors

### Step 5: Resource Assessment

Identify required:

- Technology
- Infrastructure
- Personnel
- Training
- Budget considerations

### Step 6: Barrier Assessment

Identify:

- Adoption barriers
- Workflow friction
- Technical limitations
- Organizational resistance
- Resource constraints

### Step 7: Success Metrics

Extract or infer:

- Clinical KPIs
- Operational KPIs
- Adoption KPIs
- Patient outcome metrics

### Step 8: Implementation Roadmap

Generate:

- 30-Day Plan
- 60-Day Plan
- 90-Day Plan

Each phase must contain:

- Objectives
- Key activities
- Owners
- Deliverables

## Key Concepts

| Concept | Definition |
|---------|------------|
| Recommendation Priority | High: strong evidence + impact + feasibility; Medium: moderate evidence or effort; Low: lower urgency/impact or longer dependency. |
| Barrier Risk Level | High: likely to block adoption; Medium: material impact without mitigation; Low: limited impact and straightforward mitigation. |
| Evidence Confidence | High: explicit source support; Medium: inferred from multiple signals; Low: limited or unclear support. |

When evidence is incomplete, state assumptions explicitly and continue with
the most defensible interpretation.

## Tools & Systems

| Input Artifact | Purpose |
|----------------|---------|
| Clinical guideline | Source of explicit recommendations and standards of care |
| Research paper | Evidence quality, effect direction, implementation considerations |
| HTA / product evaluation report | Technology feasibility, cost and operational readiness signals |
| Clinical implementation report | Real-world barriers, outcomes, and rollout constraints |

## Common Scenarios

- Hospital leadership needs a 30-60-90 day implementation brief from a guideline.
- Clinical operations needs a stakeholder map and barrier assessment before rollout.
- Digital health teams need measurable adoption and outcomes KPIs from evidence.

## Output Format

Produce output using this exact structure:

# Clinical Implementation Brief

## Context Profile & Assumptions

### Confirmed Institution Inputs

...

### Assumptions (if any)

| Assumption | Why Needed | Confidence | Validation Needed |
|------------|------------|------------|-------------------|

## Executive Summary

Provide a concise overview.

## Key Recommendations

| Recommendation | Priority | Rationale |
|---------------|----------|-----------|

## Stakeholder Map

### Primary Stakeholders

...

### Secondary Stakeholders

...

## Resource Requirements

### Technology

...

### Personnel

...

### Training

...

## Risk & Barrier Assessment

| Barrier | Impact | Mitigation |
|---------|--------|------------|

## Success Metrics

### Clinical Metrics

...

### Operational Metrics

...

### Adoption Metrics

...

## 30-60-90 Day Implementation Roadmap

### First 30 Days

...

### Days 31-60

...

### Days 61-90

...

## Verification

Before finalizing, confirm:

- Institution-specific context was collected before planning.
- Any missing context is captured as explicit assumptions.
- All major recommendations were extracted.
- Stakeholders were identified.
- Resource requirements were assessed.
- Risks were documented.
- Success metrics were proposed.
- Roadmap includes actionable next steps.

If any section cannot be completed from available evidence, explicitly state
assumptions and confidence level.
