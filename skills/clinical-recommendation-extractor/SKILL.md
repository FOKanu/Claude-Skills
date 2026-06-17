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

## Workflow

### Step 1: Clinical Objective

Determine:

- Primary problem addressed
- Target population
- Intended outcomes

### Step 2: Recommendation Extraction

Identify:

- Explicit recommendations
- Implicit recommendations
- Best-practice guidance
- Required workflow changes

### Step 3: Stakeholder Identification

Identify all relevant stakeholders:

- Physicians
- Nurses
- Clinical leadership
- IT teams
- Biomedical engineering
- Operations
- Patients
- External vendors

### Step 4: Resource Assessment

Identify required:

- Technology
- Infrastructure
- Personnel
- Training
- Budget considerations

### Step 5: Barrier Assessment

Identify:

- Adoption barriers
- Workflow friction
- Technical limitations
- Organizational resistance
- Resource constraints

### Step 6: Success Metrics

Extract or infer:

- Clinical KPIs
- Operational KPIs
- Adoption KPIs
- Patient outcome metrics

### Step 7: Implementation Roadmap

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

- All major recommendations were extracted.
- Stakeholders were identified.
- Resource requirements were assessed.
- Risks were documented.
- Success metrics were proposed.
- Roadmap includes actionable next steps.

If any section cannot be completed from available evidence, explicitly state
assumptions and confidence level.
