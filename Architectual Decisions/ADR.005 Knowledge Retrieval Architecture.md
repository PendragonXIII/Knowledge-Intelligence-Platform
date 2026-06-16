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

## Repository Model

The Git Repository remains the authoritative source of truth.

Knowledge Objects are stored as Markdown documents.

Relationships are represented through Obsidian links.

Examples:

[[EID.08 Knowledge Intelligence]]

[[OP.012 Knowledge Retrieval Service]]

[[CNS.005 Knowledge Object Standards]]

## Parsing Strategy

The Retrieval Service shall parse:

- document identifiers
- document titles
- object types
- section content
- Obsidian links
- relationship references

The service shall identify relationships through Obsidian link syntax.

Example:

[[EID.08 Knowledge Intelligence]]

The parser shall extract:

Identifier:
EID.08

Title:
Knowledge Intelligence

Relationship Type:
Knowledge Object Reference

## Retrieval Scope

The Retrieval Service shall support:

### Object Retrieval

Retrieve a Knowledge Object by identifier.

Examples:

- EID.08
- OP.001
- ADR.004

### Relationship Retrieval

Retrieve Knowledge Objects related to a specified object.

Examples:

- Related Capabilities
- Related Opportunities
- Related Constraints
- Related Playbooks

### Context Retrieval

Retrieve a contextual collection of related Knowledge Objects.

Examples:

- Capability Context
- Governance Context
- Opportunity Context

### Repository Navigation

Support traversal of repository relationships through Knowledge Graph operations.

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

Edges:

- Related
- Depends On
- Governs
- Supports
- References

The Knowledge Graph shall be updated whenever repository changes are processed.

## Service Interfaces

The Retrieval Service shall expose interfaces for:

Object Retrieval

GET /object/{id}

Relationship Retrieval

GET /related/{id}

Context Retrieval

GET /context/{id}

Repository Search

GET /search

Graph Retrieval

GET /graph/{id}

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

Markdown and Obsidian links are already:

- human-readable
- AI-readable
- repository-native
- governance-compatible

Introducing a frontmatter-based metadata model would require repository-wide migration without providing sufficient additional value.

The chosen approach preserves:

- existing repository investments
- Obsidian compatibility
- governance consistency
- implementation simplicity

## Consequences

The Retrieval Service becomes the foundation for:

- Search
- Validation
- Governance Review
- Knowledge Object Creation
- Knowledge Object Update
- Context Assembly

Future capabilities shall build upon the retrieval architecture defined by this ADR.

## Related Capabilities

[[EID.08 Knowledge Intelligence]]

[[EID.03 Context Intelligence]]

[[EID.07 Validation Intelligence]]

## Related Opportunities

[[OP.001 Knowledge Intelligence Service]]

[[OP.012 Knowledge Retrieval Service]]

[[OP.013 Knowledge Search Service]]

[[OP.014 Knowledge Validation Service]]

## Related Constraints

[[CNS.001 Knowledge Source of Truth]]

[[CNS.005 Knowledge Object Standards]]

[[CNS.006 Git-Managed Knowledge Repository]]

## Related ADRs

[[ADR.004 Knowledge Intelligence Service Architecture]]