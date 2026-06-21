## Status

Accepted

## Context

Architecture Decision Records influence Knowledge Graph traversal, context assembly and AI reasoning.

Traditional ADR status handling does not sufficiently address Knowledge Graph retrieval and limited traversal depth.

A lifecycle and resolution strategy is required.

## Decision

ADRs shall support the following lifecycle states:

- Proposed
- Accepted
- Historical
- Deprecated
- Superseded

## Resolution Rules

### Accepted

Represents current architectural guidance.

### Historical

Represents historically important decisions.

Historical ADRs remain discoverable but are not treated as active guidance.

### Deprecated

Represents decisions that should no longer be followed.

### Superseded

Represents decisions replaced by newer ADRs.

## Retrieval Rules

For active guidance:

- Accepted ADRs take precedence.
- Superseded chains should resolve to the latest Accepted ADR.

For historical analysis:

- Historical ADRs remain visible.
- Superseded ADRs remain visible.

## Rationale

Preserves architecture history while ensuring current guidance remains discoverable.

## Related

[[ADR.001 Knowledge Intelligence belongs to Engineering Intelligence]]

[[ADR.008 Assistant-Specific Capability Domains]]