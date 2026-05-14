# PMCOCO Requirement Workflow

A standalone Codex skill for turning workspace-based raw requirement materials into handoff-ready outputs for design and development.

## What this skill does

This skill applies a layered requirement analysis and solution design workflow:

1. Goals and scope
2. Roles and workflows
3. Data sources and structured fields
4. System flow, modules, states, and acceptance

It is designed to work even when other PM or writing-related skills are not installed.

## Best-fit scenarios

This skill works best when requirement analysis is not created from a blank page, but converged from existing workspace artifacts.

Typical best-fit scenarios include:

- A project folder already contains raw requirement notes, draft PRD files, task-design files, research notes, or meeting outputs
- The team needs to turn scattered materials into a handoff-ready design and development document
- The project is in demo, PoC, or MVP phase and needs a minimum closed-loop design rather than a large complete product definition
- The analysis must reflect roles, workflows, data lineage, and downstream collaboration rather than only feature descriptions

## Recommended upstream inputs

The following types of files or inputs are especially helpful:

- Raw requirement documents describing the business request or idea
- Existing PRD drafts in markdown, docx-exported text, or rtf-exported text
- Task design documents that already break down data-source, integration, or implementation concerns
- Research notes, meeting notes, workshop notes, or analyst summaries
- Structured source references such as spreadsheets, data-source lists, sample records, or field mappings
- Any previous intermediate outputs that reflect role design, workflow thinking, or module assumptions

## Recommended context order

1. The main raw requirement document or project request
2. The latest available PRD or structured draft
3. Any task-design or data-source design document
4. Meeting notes, workshop notes, or research artifacts
5. Supporting spreadsheets, source lists, sample data, or field definitions

If only one input can be given, the best choice is usually the most recent structured requirement document. If multiple inputs are available, the best results usually come from combining the raw request, the latest structured draft, and at least one data/task design artifact.

## Folder structure

- `SKILL.md`: main workflow instructions
- `agents/openai.yaml`: UI metadata
- `references/workflow-method.md`: full method description
- `references/dependency-review.md`: standalone packaging rationale
- `references/handoff-checklist.md`: downstream handoff validation checklist
- `assets/output-template.md`: recommended output structure

## How to use

Place this folder under your local Codex skills directory, then invoke it explicitly in a new conversation.

Example:

`Use $pmcoco-requirement-workflow to analyze the current workspace requirement documents and produce a handoff-ready output for design and development.`

## Notes

This package intentionally bundles the essential method and templates directly, instead of assuming external product or writing skills are installed.
