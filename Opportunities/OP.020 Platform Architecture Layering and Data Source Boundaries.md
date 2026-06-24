# OP.020 Platform Architecture Layering and Data Source Boundaries

## Purpose

Explicitly document the architectural separation between the Governance Core and Business Solution layers.

## Problem

Assistants may incorrectly assume that business solution operational data is stored within the Governance Core repository.

This can lead to incorrect conclusions regarding:

- data availability
- repository completeness
- solution capabilities
- system boundaries
- ownership responsibilities

## Architectural Finding

The platform contains at least two fundamentally different concerns.

### Governance and Documentation Core

Purpose:

- standards
- playbooks
- governance
- assistant profiles
- architecture
- learnings
- opportunities
- engineering guidance

This layer supports and governs solutions.

It is not intended to contain operational business data.

### Business Solution Layer

Purpose:

- domain functionality
- operational workflows
- domain reasoning
- solution execution

Examples:

- Garden Assistant
- Cooking Assistant
- Legal Assistant
- Future domain assistants

Business solutions may maintain independent:

- repositories
- knowledge graphs
- databases
- document stores
- systems of record

## Opportunity

Define and document:

1. Platform architecture layers.
2. System boundaries.
3. Repository responsibilities.
4. Assistant responsibilities.
5. Data source ownership.
6. Relationships between Governance Core and Business Solutions.

## Candidate Deliverables

Potential outputs may include:

- Platform Architecture Model
- Solution Layer Model
- Data Source Architecture
- Assistant Responsibility Matrix
- Repository Responsibility Matrix

## Expected Benefits

- Reduced repository scope ambiguity
- Improved assistant reasoning
- Better architecture understanding
- Reduced incorrect assumptions
- Clearer data source identification
- Easier onboarding of future solutions
- Better separation of governance and operational concerns

## Strategic Relevance

This opportunity affects not only the Garden Assistant but all current and future business solutions.

Examples:

- Garden Assistant
- Cooking Assistant
- Legal Assistant
- Finance Assistant
- Future assistants

## Status

Proposed

## Related

[[LRN.018 Governance Core vs Business Solution Data Separation]]

[[ASP.001 Knowledge Assistant Profile]]

[[PLB.000 Knowledge Session Initialization]]