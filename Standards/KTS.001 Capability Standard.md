## Purpose

Define the standard structure and governance requirements for Capability knowledge objects.

## Capability Domains

Capabilities shall belong to a capability domain.

Supported domains:

- EID.xxx = Engineering Intelligence Domain
- KID.xxx = Knowledge Intelligence Domain
- GID.xxx = Garden Intelligence Domain

Capability ownership shall align with ADR.008 Assistant-Specific Capability Domains.

## Human-Centered Capability Design

Capability governance should consider both system objectives and human usability needs.

Decision support, navigation, prioritization, visualization and cognitive accessibility may influence capability design and evaluation.

## Mandatory Fields

- Purpose
- Current State
- North Star
- Outcomes
- Related

## Recommended Fields

- Agentic Contribution
- Related Opportunities
- Related Constraints
- Capability Domain

## Optional Fields

- Scope
- Consumers
- Human Need

## Validation Rules

### V1
Every Capability must have a unique identifier.

### V2
Every Capability must follow KTS.001.

### V3
Every Capability must reference at least one related Opportunity.

### V4
Every Capability should maintain at least three meaningful relationships.

### V5
Mandatory fields must be present.

### V6
Recommended fields should be completed whenever sufficient information exists.

### V7
Optional fields may be omitted.

### V8
Capability identifier prefix must match the owning capability domain.

### V9
Capability design should consider relevant human usability requirements when applicable.

## Template

### Purpose

### Capability Domain

### Current State

### North Star

### Agentic Contribution

### Human Need

### Outcomes

#### O1

#### O2

#### O3

### Scope

#### In Scope

#### Out of Scope

### Consumers

### Related Opportunities

### Related Constraints

### Related

## Related

[[ADR.008 Assistant-Specific Capability Domains]]

[[ADR.010 Knowledge Planning Precedes Engineering Execution]]

[[LRN.012 Human Needs Influence Knowledge Design]]

[[KTS.010 Knowledge Object Identifier Standard]]

[[KTS.000 Knowledge Standard]]