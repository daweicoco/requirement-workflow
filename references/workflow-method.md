# PMCOCO Workflow Method

## Positioning

This workflow is not a generic PM writing prompt and not a single-document PRD template.

It is a reusable requirement analysis and solution design method for project work conducted inside a specific local workspace.

Its purpose is to convert raw requirement materials into outputs that downstream design and development teams can continue from directly.

## Core ideas

- Focus on roles, not only functions
- Focus on closed-loop workflows, not only pages
- Focus on data lineage, not only display content
- Focus on handoff-ready collaboration, not only expression
- Use layered convergence rather than flat expansion

## Layered convergence sequence

1. Goals and scope first
2. Roles and workflows next
3. Data sources and structured fields next
4. System flow, modules, states, and acceptance last

## Goals and scope

Before writing any module or page-level content, identify:

- current project stage
- immediate goals
- scope boundaries
- non-goals
- success criteria

## Roles and workflows

Define users by role and write workflows separately for each meaningful role.

Each workflow should make clear:

- trigger
- main actions
- system actions
- result
- end condition

## Data sources and structured fields

For every workflow, identify the required data support.

At minimum clarify:

- source list
- source acquisition or integration method
- raw-to-structured relation
- structured field list
- field usage in filtering, routing, display, and tracking
- traceability back to source

## System flow, modules, states, and acceptance

After the upper layers are stable, finalize:

- end-to-end system flow
- module breakdown
- responsibilities
- state transitions
- acceptance criteria
- risks and development notes

## Handoff orientation

A finished output should support at least the following downstream tasks:

- design: page inventory, flow design, interaction clarification
- engineering: modules, interfaces, data structures, rules implementation
- testing: scenario coverage, state verification, acceptance validation
