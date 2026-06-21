# ADR.010 Knowledge Planning Precedes Engineering Execution

## Status

Accepted

## Context

Knowledge work and engineering work represent distinct activities with different objectives.

Knowledge activities focus on:

- capability identification
- prioritization
- governance
- roadmap alignment
- decision support

Engineering activities focus on:

- implementation planning
- architecture realization
- testing
- deployment

Experience demonstrated that implementation quality improves when knowledge decisions are established before engineering execution begins.

## Decision

Knowledge planning shall precede engineering execution.

The Knowledge Assistant is responsible for determining:

- what should be built
- why it should be built
- priority and sequencing
- capability alignment

The Engineering Assistant is responsible for determining:

- how it should be built
- implementation approach
- validation strategy
- technical execution

Engineering work should begin from validated knowledge artifacts whenever available.

## Rationale

This separation:

- improves decision quality
- reduces implementation churn
- improves prioritization
- strengthens governance
- supports assistant specialization

## Implications

Knowledge outputs may be transferred into engineering activities through:

- Capabilities
- Roadmaps
- ADRs
- Engineering Handoffs

Engineering sessions should consume knowledge outputs rather than recreate strategic decisions.

## Related

[[LRN.013 Knowledge Work Precedes Engineering Work]]

[[ASP.001 Knowledge Assistant Profile]]

[[ASP.002 Engineering Assistant Profile]]

[[KTS.011 Engineering Handoff Standard]]