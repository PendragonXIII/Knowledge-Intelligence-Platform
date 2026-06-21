## Status

Superseded

## Superseded By

[[ADR.008 Assistant-Specific Capability Domains]]

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

Its responsibilities naturally extend existing Engineering Intelligence capabilities.

## Implications

- Engineering Intelligence becomes the parent domain for Knowledge Intelligence.
- Knowledge Intelligence becomes EID.08.

## Related

[[ADR.008 Assistant-Specific Capability Domains]]

[[EID.08 Knowledge Intelligence]]