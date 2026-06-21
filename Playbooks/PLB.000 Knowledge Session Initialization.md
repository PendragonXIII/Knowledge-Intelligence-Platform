# PLB.000 Knowledge Session Initialization

## Purpose

Establish the minimum governance, roadmap and operational context required before executing Knowledge Management activities.

The objective is to ensure that Knowledge Assistants begin each session with sufficient context while avoiding unnecessary repository loading.

## Principles

- Load context before analysis.
- Load only the context required for the current session.
- Prefer repository knowledge over GPT instructions.
- Use specialized playbooks for specialized activities.
- Explicitly load deeper context when relationships extend beyond the default traversal depth.
- Load the active Assistant Profile before beginning substantive work.

## Context Loading Strategy

### Layer 1 – Foundation Context

Load first:

- KTS.000 Knowledge Standard
- Current Knowledge Object Standards (KTS)
- Current Knowledge Object Types
- Active Assistant Profile (ASP)

Purpose:

Establish governance rules, object taxonomy and assistant behavior.

### Layer 2 – Strategic Context

Load:

- Active Roadmaps
- Major Capabilities
- Current foundational Learnings

Purpose:

Establish current repository direction and strategic priorities.

### Layer 3 – Session Classification

Determine the primary session type.

Possible classifications:

- Knowledge Creation
- Knowledge Review
- Governance Review
- Architecture Review
- Roadmap Planning
- Capability Development
- Repository Maintenance

## Assistant Profile Selection

Identify and load the Assistant Profile associated with the current assistant.

Examples:

- Knowledge Assistant → ASP.001
- Engineering Assistant → ASP.002
- Garden Assistant → ASP.003

Assistant Profiles govern:

- reasoning behavior
- communication style
- visualization preferences
- context loading preferences
- session behavior

## Playbook Selection

After classification, load the most relevant specialized playbook.

Examples:

- Knowledge Object Creation → PLB.003
- Knowledge Object Assessment → PLB.004
- Knowledge Session Initialization → PLB.000

## Deep Context Rule

Knowledge retrieval may be limited by default relationship traversal depth.

When important context appears to exist beyond currently loaded relationships:

- explicitly load additional referenced objects
- continue loading until sufficient context exists for the requested activity
- do not assume absence of context implies absence of knowledge

## Session Output Requirements

Before producing recommendations, reviews or governance decisions, verify that:

- foundational standards have been considered
- relevant playbooks have been loaded
- active assistant profile has been loaded
- strategic context has been reviewed
- required related objects have been examined

## Success Criteria

A session is considered initialized when:

- governance context is loaded
- assistant profile is loaded
- strategic context is loaded
- session type is identified
- specialized playbook is selected
- additional context requirements are known

## Related

[[KTS.000 Knowledge Standard]]

[[KTS.009 Assistant Profile Standard]]

[[ASP.001 Knowledge Assistant Profile]]

[[ASP.002 Engineering Assistant Profile]]

[[ASP.003 Garden Assistant Profile]]

[[PLB.003 Knowledge Object Creation]]

[[PLB.004 Knowledge Object Assessment]]

[[EID.08 Knowledge Intelligence]]