## Status

Accepted

## Context

The Knowledge Intelligence Service requires a standardized mechanism for retrieving Knowledge Objects from the Knowledge Repository.

The repository is maintained as a Git-managed collection of Markdown documents authored through Obsidian.

Knowledge Objects contain structured sections and explicit relationships using Obsidian-style links.

Examples:

[[EID.08 Knowledge Intelligence]]

[[OP.001 Knowledge Intelligence Service]]

Future AI systems require the ability to:

- retrieve Knowledge Objects
- discover related Knowledge Objects
- assemble contextual information
- traverse repository relationships

without requiring direct repository access.

A retrieval architecture is required before search, validation, creation and update capabilities can be implemented.

## Decision

Implement a Knowledge Retrieval Service as the first operational capability of the Knowledge Intelligence Service.

The service shall:

- retrieve Knowledge Objects from the Git Repository
- parse Markdown content
- parse Obsidian relationships
- expose retrieval functionality through FastAPI endpoints

The service shall use Markdown and Obsidian link parsing as the authoritative retrieval mechanism.

No frontmatter-based metadata model shall be introduced.

## Knowledge Graph Integration

Knowledge Objects and relationships shall be transformed into a persistent Knowledge Graph.

The Knowledge Graph shall contain:

Nodes:

- Capabilities
- Opportunities
- Constraints
- Learnings
- ADRs
- Playbooks
- Roadmaps
- Standards
- Assistant Profiles

Edges:

- Related
- Depends On
- Governs
- Supports
- References

The Knowledge Graph shall be updated whenever repository changes are processed.

## Retrieval Scope

The Retrieval Service shall support:

- Object Retrieval
- Relationship Retrieval
- Context Retrieval
- Repository Navigation

## Responsibilities

### Retrieval Service

Responsible for:

- repository access
- Markdown parsing
- Obsidian link parsing
- relationship extraction
- graph synchronization
- context assembly

### Knowledge Repository

Responsible for:

- knowledge persistence
- relationship persistence
- governance compliance

### Custom GPT

Responsible for:

- reasoning
- interpretation
- recommendations
- workflow orchestration

The Custom GPT shall consume retrieval services rather than directly accessing repository contents.

## Rationale

Markdown and Obsidian links are:

- human-readable
- AI-readable
- repository-native
- governance-compatible

## Consequences

The Retrieval Service becomes the foundation for:

- Search
- Validation
- Governance Review
- Knowledge Object Creation
- Knowledge Object Update
- Context Assembly

Future capabilities shall build upon the retrieval architecture defined by this ADR.

## Related

[[ADR.004 Knowledge Intelligence Service Architecture]]

[[ASP.001 Knowledge Assistant Profile]]

[[ASP.002 Engineering Assistant Profile]]

[[ASP.003 Garden Assistant Profile]]