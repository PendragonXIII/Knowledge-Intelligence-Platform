## Status

Accepted

## Context

The objective is to improve AI context quality, recommendation consistency and engineering effectiveness.

A knowledge layer is required to capture capabilities, opportunities, constraints, playbooks, learnings and architectural decisions.

The value resides in the knowledge itself, not in a specific tool.

## Decision

Obsidian shall be used as the primary authoring environment for the Knowledge Layer.

The Knowledge Layer shall remain independent from Obsidian as a technology.

Knowledge artifacts shall remain Markdown-based and portable.

## Rationale

Obsidian provides:

- efficient knowledge authoring
- knowledge graph visualization
- relationship discovery
- mobile and desktop usability
- Git compatibility

The long-term goal is not Obsidian integration.

The long-term goal is AI consumption of structured knowledge.

## Implications

- Obsidian is an editor, not the knowledge itself.
- Knowledge artifacts should remain tool-independent.
- Git remains the long-term storage and versioning mechanism.
- Future AI assistants should consume knowledge without requiring direct Obsidian integration.
- Knowledge objects should be portable across tools and platforms.

## Alternatives Considered

### Repository-Only Knowledge

Rejected because relationship management and knowledge discovery are limited.

### Obsidian as System of Record

Rejected because it introduces unnecessary tool dependency.

## Related

[[ADR.001 Knowledge Intelligence belongs to Engineering Intelligence]]

[[CNS.001 Knowledge Source of Truth]]

[[CNS.003 Avoid Duplicate Knowledge Ownership]]

[[CNS.004 Knowledge Must Remain AI Consumable]]

[[EID.08 Knowledge Intelligence]]

[[OP.001 Knowledge Layer Assistant]]