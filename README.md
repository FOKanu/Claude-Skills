# Claude Skills Portfolio

This repository contains two production-ready, domain-specific Claude skills designed for structured execution, repeatable outputs, and real-world team workflows.

The goal is simple: move from generic prompting to reusable operational playbooks that an AI agent can execute consistently.

## Skills Included

### `clinical-recommendation-extractor`

Converts healthcare evidence (guidelines, research, implementation reports) into implementation-ready outputs:

- Prioritized recommendations
- Stakeholder maps
- Resource requirements
- Risk and barrier assessment
- 30-60-90 day roadmap
- Verification checklist

Primary use case: helping healthcare, digital health, and MedTech teams operationalize evidence quickly and responsibly.

### `meeting-intelligence-action-tracker`

Converts unstructured meeting artifacts (transcripts, notes, workshop output) into execution-focused documentation:

- Decision logs
- Action items with owner and due date structure
- Risks and blockers
- Outstanding questions
- Next meeting agenda
- Verification checklist

Primary use case: improving accountability and execution quality across project, product, and operations teams.

## Skill Format Used

Each skill follows a standard skill-directory pattern:

```text
skills/<skill-name>/
└── SKILL.md
```

Each `SKILL.md` includes:

1. YAML frontmatter for discovery and indexing:
   - `name`
   - `description`
   - `domain`
   - `subdomain`
   - `tags`
   - `version`
   - `author`
   - `license`
2. Structured markdown sections for execution:
   - `When to Use`
   - `When Not to Use`
   - `Prerequisites`
   - `Workflow`
   - `Key Concepts`
   - `Tools & Systems`
   - `Common Scenarios`
   - `Output Format`
   - `Verification`

This format improves reliability because the agent can decide when to invoke the skill, follow an explicit process, and deliver consistent outputs.

## Why This Format

This structure is intentionally aligned with current industry patterns for high-quality agent skills:

- Metadata-driven discovery (fast filtering by domain/subdomain/tags)
- Workflow-driven execution (clear sequence, fewer hallucinated steps)
- Contract-driven outputs (predictable format for downstream users)
- Verification-first quality control (explicit completeness checks)

In practical terms, this makes the skills usable in enterprise contexts where consistency, traceability, and handoff quality matter more than one-off prompt creativity.

## Research and Design Approach

These skills were developed after reviewing open-source skill ecosystems and enterprise-oriented skill conventions to ensure stronger operational quality.

The design approach emphasized:

- Reusable task decomposition over freeform prompting
- Clear decision criteria and confidence signaling
- Actionable deliverables that a manager or team lead can use immediately
- Taxonomy normalization (`domain`, `subdomain`, `tags`) for long-term maintainability

This research-informed approach reflects how teams are increasingly productionizing AI support: by encoding expert workflows into stable, versioned skill assets.

## Recruiter / Hiring Manager Relevance

This repository demonstrates applied strengths in:

- AI workflow design and prompt systems engineering
- Knowledge operationalization (turning messy input into executable plans)
- Product-minded documentation and output contracts
- Enterprise readiness (repeatability, governance, auditability)

Rather than showcasing isolated prompts, this work shows how to build AI capabilities that can be adopted by teams, scaled across use cases, and maintained over time.

## License

Apache-2.0 (per-skill metadata).
