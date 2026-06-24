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
Governance Verification
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

## Governance Verification

Before substantive analysis or execution begins verify:

1. Active Assistant Profile has been loaded.
2. Governing Playbook has been loaded when available.
3. Required standards have been reviewed.
4. Repository Resolution Validation has been completed.
5. Required repository evidence has been loaded.
6. Required context has been reviewed.

Loaded governance shall be explicitly verified before execution.

Governance assumed but not verified shall not be treated as active context.

## Activity Transition Validation

When the activity type changes during a session:

1. Identify the new activity.
2. Determine the governing Playbook for the new activity.
3. Perform Governance Verification for the new activity.
4. Initialize the new activity before execution.

Examples:

- Review → Modification
- Assessment → Creation
- Analysis → Repository Update
- Discovery → ADR Creation

Findings and recommendations may lead to new activities.

Recommendations shall not automatically trigger repository modifications.

Repository modifications require explicit activation of the governing modification Playbook.

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
6. Verify governance context.
7. Execute activity.

### Knowledge Object Lifecycle

- Create new knowledge object → PLB.003 Knowledge Object Creation
- Modify existing knowledge object → PLB.013 Knowledge Object Modification

## Session Output Requirements

Before execution verify:

- assistant profile loaded
- governing playbook loaded
- repository resolution validated
- governance verified
- repository evidence reviewed
- required context reviewed

## Success Criteria

A session is initialized when:

- assistant profile is loaded
- activity is identified
- governing playbook is identified
- governing playbook is loaded
- repository resolution is validated
- governance is verified
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