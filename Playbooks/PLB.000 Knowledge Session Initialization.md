# PLB.000 Knowledge Session Initialization

## Purpose

Establish the minimum governance and operational context required before executing Knowledge Management activities.

## Principles

- Load repository evidence before interpretation.
- Load context before analysis.
- Prefer repository knowledge over GPT instructions.
- Load the active Assistant Profile before substantive work.
- Governed activities should be executed through their corresponding Playbooks.

## Initialization Flow

Activity Identification
↓
Assistant Profile Selection
↓
Playbook Identification
↓
Playbook Loading
↓
Repository Evidence Loading
↓
Context Expansion
↓
Execution

## Repository-First Interpretation

For governance, architecture, taxonomy, capability ownership, object semantics and repository structure:

Repository artifacts should be loaded before interpretation begins.

Preferred sequence:

Repository Evidence
↓
Analysis
↓
Recommendation

## Context Loading Strategy

### Layer 1 – Foundation Context

Load:

- KTS.000 Knowledge Standard
- Current Knowledge Object Standards
- Active Assistant Profile

### Layer 2 – Repository Evidence

Load repository artifacts required by the active Playbook.

### Layer 3 – Strategic Context

Load:

- Active Roadmaps
- Major Capabilities
- Relevant ADRs
- Relevant Learnings

### Layer 4 – Session Classification

Identify the primary activity and session type.

## Assistant Profile Selection

- Knowledge Assistant → ASP.001
- Engineering Assistant → ASP.002
- Garden Assistant → ASP.003

## Playbook Identification

For every governed activity:

1. Identify activity type.
2. Identify governing Playbook.
3. Load Playbook.
4. Load repository evidence required by the Playbook.
5. Execute activity.

## Session Output Requirements

Before execution verify:

- assistant profile loaded
- governing playbook loaded
- repository evidence reviewed
- required context reviewed

## Success Criteria

A session is initialized when:

- assistant profile is loaded
- activity is identified
- governing playbook is identified
- governing playbook is loaded
- repository evidence is loaded
- required context is available

## Related

[[LRN.015 Playbook-Driven Execution]]

[[LRN.016 Repository-First Interpretation]]

[[ASP.001 Knowledge Assistant Profile]]

[[ASP.002 Engineering Assistant Profile]]

[[ASP.003 Garden Assistant Profile]]