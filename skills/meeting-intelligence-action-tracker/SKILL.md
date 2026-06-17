---
name: meeting-intelligence-action-tracker
description: >
  Transform raw meeting transcripts, notes, brainstorming sessions,
  and workshop outputs into structured meeting minutes, action items,
  decisions, risks, ownership assignments, and follow-up plans.
domain: business-operations
subdomain: meeting-intelligence
tags:
  - business-operations
  - meetings
  - project-management
  - action-tracking
  - productivity
version: "1.0.0"
author: Francis I.K.
license: Apache-2.0
---

# Meeting Intelligence & Action Tracker

## When to Use

Use this skill when the user provides:

- Meeting notes
- Meeting transcripts
- Workshop notes
- Brainstorming sessions
- Interview notes
- Stakeholder discussions
- Project update meetings

## When Not to Use

Do not use this skill for:

- Legal transcription
- Verbatim meeting records
- Audio processing
- Translation tasks

## Prerequisites

The user should provide one or more of:

- Raw meeting transcript
- Meeting notes or facilitator notes
- Participant list (if available)
- Any known deadlines, owners, or decision logs

If critical information is missing, continue extraction and mark unknown fields
explicitly as not specified.

## Workflow

### Step 1: Meeting Context

Identify:

- Meeting purpose
- Participants
- Main discussion topics

### Step 2: Decision Extraction

Identify:

- Explicit decisions
- Implicit decisions
- Approved proposals
- Rejected proposals

### Step 3: Action Item Extraction

For each action item determine:

- Task
- Owner
- Due date
- Dependencies

If owner or deadline is missing, mark as:

- Owner Not Specified
- Deadline Not Specified

### Step 4: Risk Identification

Identify:

- Open concerns
- Blockers
- Resource limitations
- Technical risks
- Operational risks

### Step 5: Follow-Up Requirements

Identify:

- Outstanding questions
- Pending decisions
- Required approvals
- Additional stakeholders

### Step 6: Next Meeting Preparation

Generate:

- Proposed agenda
- Key decisions required
- Outstanding action items

## Key Concepts

| Concept | Definition |
|---------|------------|
| Decision Confidence | High: explicit and agreed; Medium: implied by aligned statements; Low: inferred from ambiguous discussion. |
| Action Item Completeness | Complete: task + owner + due date; Partial: one missing key field; Incomplete: owner and due date missing. |
| Risk Severity | High: immediate blocker or major impact; Medium: credible delay/quality risk; Low: manageable issue with limited impact. |

When uncertainty exists, preserve traceability by flagging assumptions.

## Tools & Systems

| Input Artifact | Purpose |
|----------------|---------|
| Meeting transcript | Primary source for decisions, actions, risks, and rationale |
| Notes / facilitator notes | Fill context gaps and improve accuracy of extraction |
| Participant list | Clarify ownership and role mapping in action items |
| Deadline or decision logs | Validate due dates and unresolved decisions |

## Common Scenarios

- Weekly project stand-up requires clean minutes and owner-assigned actions.
- Cross-functional workshop needs explicit decisions and unresolved questions captured.
- Steering committee meeting needs blockers, mitigation, and next-agenda handoff.

## Output Format

Produce output using this exact structure:

# Meeting Minutes

## Executive Summary

...

## Participants

| Name | Role |
|------|------|

## Key Discussion Topics

...

## Decisions Made

| Decision | Rationale |
|----------|-----------|

## Action Items

| Task | Owner | Due Date | Status |
|------|-------|----------|--------|

## Risks & Blockers

| Issue | Impact | Mitigation |
|-------|--------|------------|

## Outstanding Questions

...

## Next Meeting Agenda

1.
2.
3.

## Verification

Before finalizing verify:

- All decisions captured
- All action items captured
- Owners identified
- Deadlines identified
- Risks documented
- Outstanding questions documented

If information is missing, explicitly indicate uncertainty.
