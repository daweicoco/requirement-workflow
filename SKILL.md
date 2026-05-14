---
name: requirement-workflow
description: Structured requirement analysis and solution design workflow for local workspace-based product work. Use when Codex needs to turn raw requirement documents, scattered project materials, drafts, meeting notes, or existing PRD and task-design artifacts into handoff-ready outputs for design and development. The workflow follows layered convergence: define goals and scope first, then roles and workflows, then data sources and structured fields, then system flow, modules, states, acceptance criteria, risks, and development handoff notes. This skill is designed to be standalone and should not require other product or writing skills to produce a complete result.
---

# Objective

Use the current workspace documents as the primary source of truth and produce outputs that are ready for downstream collaboration.

This skill is not a generic PRD-writing helper. It is a handoff-oriented requirement analysis and solution design workflow.

# Source-of-truth rule

Always prioritize local workspace materials over general assumptions.

Read in this order when available:

1. User-specified files in the current workspace
2. Existing project PRD, task design, research, notes, and related artifacts
3. Related drafts in markdown, docx-exported text, rtf-exported text, spreadsheets, or auxiliary outputs
4. Bundled references and templates in this skill

Do not rely on external skills. If similar methods were previously provided by other skills, reproduce the needed structure from this package directly.

# Required execution order

Follow this sequence unless the user explicitly asks for a different order:

1. Clarify project stage, goals, scope, and non-goals
2. Define user roles, responsibilities, and permission boundaries
3. Write role-specific workflows and ensure flow closure
4. Identify data sources, structured fields, and data lineage
5. Design the end-to-end system flow
6. Break down modules and module responsibilities
7. Define states and state transitions
8. Produce acceptance criteria, risks, open questions, and development handoff notes

Do not begin with feature lists before goals and scope are clear.

# Core principles

- Prioritize roles over page lists
- Prioritize closed-loop workflows over isolated features
- Prioritize data lineage over UI-only descriptions
- Prioritize handoff-ready outputs over abstract discussion
- Use layered convergence instead of flat documentation
- Keep every section connected to downstream design and development execution

# Workflow guidance

## 1. Goals and scope

Answer:

- What problem is being solved in this round?
- What must be proven or delivered now?
- Is this a demo, PoC, MVP, or production-phase requirement?
- What is explicitly out of scope?
- What defines success for this round?

Produce:

- product positioning
- goals
- stage definition
- scope and non-goals
- success criteria

## 2. Roles and workflows

Answer:

- Who are the core users or operators?
- What is each role trying to achieve?
- What actions are triggered by the system versus the user?
- Where does each role enter and exit the flow?
- Is the workflow actually closed-loop?

Produce:

- role definitions
- role-specific permissions
- role-specific workflows
- trigger and end conditions

## 3. Data sources and structured fields

Answer:

- Where does the data originate?
- Which data is externally acquired and which is internally generated?
- Which fields are essential for filtering, routing, decision-making, display, and tracking?
- Can structured outputs be traced back to the raw source?

Produce:

- source list
- acquisition or integration method
- raw-to-structured mapping
- field list
- field purpose notes
- data quality requirements

## 4. System flow, modules, states, and acceptance

Answer:

- What is the end-to-end business and system chain?
- Which modules are needed to carry the workflows and data?
- What responsibilities belong to each module?
- What states must be tracked?
- How will the team verify the solution is complete enough to hand off?

Produce:

- end-to-end system flow
- module breakdown
- module responsibilities
- state definitions and transitions
- non-functional requirements when relevant
- acceptance criteria
- development handoff notes

# Output requirements

Use the template in `assets/output-template.md` when a full output is needed.

A complete output should normally include:

1. Product overview
2. Goals and scope
3. User roles
4. Core workflows
5. Data sources and field design
6. End-to-end system flow
7. Functional modules
8. State design
9. Non-functional requirements if needed
10. Acceptance criteria
11. Risks and open questions
12. Development handoff notes

# Prohibitions

- Do not write feature lists before clarifying goals
- Do not merge multiple roles into one vague workflow
- Do not describe UI without supporting data and field logic
- Do not stop at conceptual language with no downstream handoff value
- Do not omit state logic when the workflow depends on progress tracking or collaboration

# References

Read `references/workflow-method.md` for the full PMCOCO method.
Read `references/dependency-review.md` for why this skill is packaged as a standalone workflow.
Read `references/handoff-checklist.md` when validating whether the output is ready for design and development.
