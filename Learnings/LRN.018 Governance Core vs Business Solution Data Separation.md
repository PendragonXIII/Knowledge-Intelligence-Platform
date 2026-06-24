# LRN.018 Governance Core vs Business Solution Data Separation

## Observation

A Garden Assistant analysis incorrectly assumed that operational garden data should exist within the Knowledge Intelligence Platform repository.

## Finding

The Knowledge Intelligence Platform repository serves as a Governance and Documentation Core.

It contains:

- Standards
- Playbooks
- Assistant Profiles
- Learnings
- Opportunities
- Architecture and governance knowledge

It is not the authoritative storage location for business solution operational data.

## Implication

Business solutions may maintain:

- independent repositories
- independent knowledge graphs
- independent operational databases
- external systems of record

Examples include:

- Garden Assistant
- Cooking Assistant
- Legal Assistant

The existence of governance artifacts for a business solution does not imply that operational domain data exists within the Governance Core repository.

## Recommendation

Assistants should explicitly distinguish between:

1. Governance and Documentation repositories.
2. Business solution repositories and operational data sources.

Repository scope should be validated before conclusions are drawn regarding data completeness.

## Related

[[PLB.000 Knowledge Session Initialization]]

[[ASP.001 Knowledge Assistant Profile]]