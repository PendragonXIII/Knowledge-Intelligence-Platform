## Status

Accepted

## Context

The existing capability model contains a substantial Engineering Intelligence ecosystem consisting of:

- Repository Intelligence
- Capability Intelligence
- Context Intelligence
- Governance Intelligence
- Risk & Decision Intelligence
- Quality Intelligence
- Validation Intelligence

Knowledge Intelligence was initially considered as a separate top-level capability.

Further architectural review showed that its primary purpose is to improve engineering reasoning, governance, context assembly and AI-assisted engineering workflows.

## Decision

Knowledge Intelligence shall be introduced as a Core Capability within the Engineering Intelligence Domain.

It shall not be introduced as an independent top-level capability.

## Rationale

Knowledge Intelligence primarily serves engineering workflows and AI-assisted engineering decision making.

Its responsibilities naturally extend existing Engineering Intelligence capabilities through:

- Knowledge Object Management
- Knowledge Relationship Management
- Knowledge Generation
- Knowledge Governance
- Knowledge Context Assembly
- Knowledge Synchronization

This placement maintains a consistent capability hierarchy and avoids introducing a top-level capability with a different aggregation level than existing Garden capabilities.

## Implications

- Engineering Intelligence becomes the parent domain for Knowledge Intelligence.
- Knowledge Intelligence becomes EID.08.
- Future knowledge-layer capabilities belong within the Engineering Intelligence Domain.
- Engineering Assistants can evolve from Repository-Aware to Knowledge-Aware systems.
- Knowledge artifacts become first-class engineering assets.

## Alternatives Considered

### Separate Top-Level Capability

Rejected because the capability scope aligns with Engineering Intelligence rather than Garden Intelligence.

### Obsidian-Centric Capability

Rejected because the capability concerns knowledge management and AI context management rather than a specific technology.

## Related

[[EID.08 Knowledge Intelligence]]

[[EID.03 Context Intelligence]]

[[EID.04 Governance Intelligence]]

[[OP.001 Knowledge Intelligence Service]]

[[OP.002 Knowledge-Aware Engineering Assistant]]