## Status

Accepted

## Context

The Garden Solution ecosystem requires a structured service layer that enables AI agents to consume knowledge stored in the Knowledge Repository.

The service must provide reliable, machine-readable access to Knowledge Objects and their relationships while remaining lightweight, cost-efficient and compatible with Railway deployment and GPT Actions.

The service acts as the operational interface between AI agents and the Git-managed Knowledge Repository.

## Decision

Establish a dedicated Knowledge Intelligence Service as a standalone FastAPI application.

The service shall:

- read Knowledge Objects from the Knowledge Repository
- resolve Knowledge Object identifiers
- extract Knowledge Relationships
- assemble Context Packs
- expose HTTP endpoints for AI consumption

The initial MVP includes:

- Retrieval Service
- Relationship Service
- Context Assembly Service
- FastAPI HTTP Interface

The initial MVP is read-only.

Write, update and governance automation capabilities are intentionally deferred.

## Rationale

The primary objective is to make the Knowledge Repository consumable by AI agents as quickly as possible.

Read capabilities provide immediate value and enable:

- Engineering Assistant integration
- Governance Assistant integration
- Garden Assistant integration
- Future AI agent integration

A read-only MVP minimizes complexity while validating the overall architecture.

## Architecture

Knowledge Repository

↓

Knowledge Intelligence Service

↓

AI Agents

↓

Engineering Assistant

↓

Garden Assistant

↓

Future Domain Assistants

The Knowledge Repository remains the Source of Truth.

The Knowledge Intelligence Service provides controlled access to repository content.

## Implemented Components

### Retrieval Layer

- RepositoryReader
- ObjectResolver
- MarkdownParser
- RetrievalService

### Knowledge Graph Layer

- RelationshipService
- ContextAssemblyService

### API Layer

- FastAPI Application
- GET /objects/{object_id}
- GET /context/{object_id}

## Testing

Automated regression testing is mandatory.

Implemented tests include:

- LinkParser
- ObjectResolver
- RepositoryReader
- MarkdownParser
- RetrievalService
- RelationshipService
- ContextAssemblyService

The MVP currently maintains a fully passing automated test suite.

## Future Enhancements

Planned future capabilities include:

- API Key Security
- Railway Deployment
- GPT Action Integration
- Search Service
- Knowledge Validation
- Knowledge Governance Automation
- Knowledge Write Capabilities
- Knowledge Update Capabilities
- Knowledge Graph Analytics

## Consequences

### Positive

- AI-consumable Knowledge Layer
- Low-cost deployment model
- Reusable architecture
- Strong governance alignment
- Incremental capability expansion

### Negative

- Read-only MVP
- No authentication in local development
- No write capabilities
- Limited graph intelligence

These limitations are accepted for the MVP phase.