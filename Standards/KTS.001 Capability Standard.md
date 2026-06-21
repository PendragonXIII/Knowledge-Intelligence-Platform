## Purpose

Define the standard structure and governance requirements for Capability knowledge objects.

## Capability Domains

Capabilities shall belong to a capability domain.

Supported domains:

- EID.xxx = Engineering Intelligence Domain
- KID.xxx = Knowledge Intelligence Domain
- GID.xxx = Garden Intelligence Domain

Capability ownership shall align with ADR.008 Assistant-Specific Capability Domains.

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

## Template

### Purpose

### Capability Domain

### Current State

### North Star

### Agentic Contribution

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

[[KTS.010 Knowledge Object Identifier Standard]]

[[KTS.000 Knowledge Standard]]