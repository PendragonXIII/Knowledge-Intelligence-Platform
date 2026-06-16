## Status

Accepted

## Context

The Knowledge Intelligence ecosystem consists of multiple logical layers.

Current and planned components include:

- Knowledge Repository
- Knowledge Intelligence Service
- Garden Assistant
- Engineering Assistant
- Future Domain Assistants

A repository strategy is required to ensure maintainability, scalability and efficient deployment.

The architecture must support:

- shared knowledge
- shared services
- multiple assistants
- low operational cost
- hobby-scale infrastructure

## Decision

Separate the ecosystem into three repositories.

Repository 1:

Knowledge Intelligence Platform

Purpose:

Knowledge storage and governance.

Repository 2:

Knowledge Intelligence Service

Purpose:

Knowledge retrieval, search, validation, graph management and repository operations.

Repository 3:

Garden Solution

Purpose:

Assistant integrations, OpenAI Actions, assistant-specific capabilities and domain workflows.

Engineering Assistant and Garden Assistant shall remain within the Garden Solution repository until independent deployment requirements emerge.

No dedicated Knowledge Assistant repository shall be created.

## Repository Responsibilities

### Knowledge Intelligence Platform

Responsible for:

- Knowledge Objects
- Knowledge Governance
- Knowledge Standards
- Knowledge Relationships
- Knowledge Graph Source Data

Examples:

- Capabilities
- Opportunities
- Constraints
- Learnings
- ADRs
- Playbooks
- Roadmaps
- Standards

### Knowledge Intelligence Service

Responsible for:

- Knowledge Retrieval
- Knowledge Search
- Knowledge Validation
- Knowledge Object Creation
- Knowledge Object Updates
- Knowledge Graph Management
- Repository Operations

The service shall expose APIs for AI systems.

### Garden Solution

Responsible for:

- Garden Assistant
- Engineering Assistant
- OpenAI Actions
- Assistant Configuration
- Domain-Specific Workflows
- Integration Logic

## Assistant Strategy

Assistants are considered consumers of knowledge rather than owners of knowledge.

Assistants shall consume Knowledge Intelligence Services rather than directly managing repository contents.

Assistants may share common infrastructure and deployment environments.

Separate assistant repositories shall not be created unless operational requirements justify separation.

## Deployment Strategy

Knowledge Intelligence Platform:

GitHub Repository

No active deployment required.

Knowledge Intelligence Service:

Railway Deployment

FastAPI Application

Garden Solution:

Railway Deployment

FastAPI Application

The architecture should remain compatible with hobby-scale infrastructure and avoid unnecessary deployment proliferation.

## Rationale

The selected approach separates:

- knowledge
- operations
- assistant behavior

while minimizing:

- deployment complexity
- infrastructure cost
- repository fragmentation

The architecture supports future growth without requiring immediate service decomposition.

## Consequences

Knowledge governance remains independent from implementation.

Knowledge services become reusable across assistants.

Future assistants can consume the same Knowledge Intelligence Service.

Infrastructure cost remains low.

Repository ownership remains clear.

## Related Capabilities

[[EID.08 Knowledge Intelligence]]

[[EID.03 Context Intelligence]]

[[EID.04 Governance Intelligence]]

## Related Opportunities

[[OP.001 Knowledge Intelligence Service]]

[[OP.012 Knowledge Retrieval Service]]

[[OP.013 Knowledge Search Service]]

[[OP.014 Knowledge Validation Service]]

[[OP.015 Knowledge Object Creation Service]]

[[OP.016 Knowledge Object Update Service]]

## Related ADRs

[[ADR.004 Knowledge Intelligence Service Architecture]]

[[ADR.005 Knowledge Retrieval Architecture]]