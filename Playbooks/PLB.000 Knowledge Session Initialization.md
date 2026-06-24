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
Repository Resolution Validation
↓
Repository Evidence Loading
↓
Context Expansion
↓
Execution

## Repository Resolution Validation

Before loading referenced repository artifacts:

1. Verify the target artifact exists.
2. Verify the expected repository location.
3. Inspect the relevant repository folder when object resolution fails.
4. Identify potential naming changes or renamed artifacts.
5. Identify candidate artifacts sharing the same identifier prefix.
6. Resolve the canonical repository path before continuing.

Repository evidence shall not be assumed to exist solely because an identifier was provided.

When ambiguity exists, repository structure takes precedence over assumptions.

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
4. Validate repository resolution for required artifacts.
5. Load repository evidence required by the Playbook.
6. Execute activity.

### Knowledge Object Lifecycle

- Create new knowledge object → PLB.003 Knowledge Object Creation
- Modify existing knowledge object → PLB.013 Knowledge Object Modification

## Session Output Requirements

Before execution verify:

- assistant profile loaded
- governing playbook loaded
- repository resolution validated
- repository evidence reviewed
- required context reviewed

## Success Criteria

A session is initialized when:

- assistant profile is loaded
- activity is identified
- governing playbook is identified
- governing playbook is loaded
- repository resolution is validated
- repository evidence is loaded
- required context is available

## Related

[[LRN.015 Playbook-Driven Execution]]

[[LRN.016 Repository-First Interpretation]]

[[PLB.003 Knowledge Object Creation]]

[[PLB.008 Knowledge Object Modification]]

[[ASP.001 Knowledge Assistant Profile]]

[[ASP.002 Engineering Assistant Profile]]

[[ASP.003 Garden Assistant Profile]]