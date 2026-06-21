## Status

Accepted

## Context

The original capability architecture was created around Engineering Intelligence.

Knowledge Intelligence was introduced as EID.08 and positioned within the Engineering Intelligence Domain through ADR.001.

Since then, the platform has evolved to support multiple assistants with distinct responsibilities:

- Engineering Assistant
- Knowledge Assistant
- Garden Assistant

Assistant Profiles (ASP) now define assistant-specific behavior, workflows and decision support patterns.

The capability landscape should evolve to reflect these assistant boundaries.

## Decision

Capability Domains shall be organized by Assistant Domain.

The following capability namespaces are established:

- EID.xxx = Engineering Intelligence Domain
- KID.xxx = Knowledge Intelligence Domain
- GID.xxx = Garden Intelligence Domain

Capabilities shall be assigned to the domain that primarily owns and evolves the capability.

## Rationale

This approach:

- aligns capabilities with assistant responsibilities
- improves discoverability
- reduces domain ambiguity
- supports future assistant expansion
- reflects the current platform architecture more accurately than a single Engineering-centric hierarchy

## Implications

- Knowledge Intelligence capabilities may migrate from EID to KID.
- Future Knowledge Assistant capabilities belong within KID.
- Future Garden Assistant capabilities belong within GID.
- Engineering-specific capabilities remain within EID.
- Capability governance should evolve to support multiple capability domains.

## Migration Strategy

1. Identify existing capabilities.
2. Determine domain ownership.
3. Reassign capabilities where appropriate.
4. Update references.
5. Validate repository consistency.

## Evolves

[[ADR.001 Knowledge Intelligence belongs to Engineering Intelligence]]

## Related

[[ASP.001 Knowledge Assistant Profile]]

[[ASP.002 Engineering Assistant Profile]]

[[ASP.003 Garden Assistant Profile]]

[[EID.08 Knowledge Intelligence]]