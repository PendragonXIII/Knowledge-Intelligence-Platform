## Purpose

Define the standard structure and governance requirements for Engineering Component knowledge objects.

Engineering Components represent implementation artifacts that realize one or more capabilities.

Engineering Components bridge the gap between governance knowledge and implementation knowledge.

Capabilities describe what a system should achieve.

Engineering Components describe how those capabilities are realized.

## Component Types

Supported component types:

- MODULE
- SERVICE
- WORKFLOW
- API
- TEST
- INTEGRATION
- INFRASTRUCTURE

## Mandatory Fields

- Purpose
- Component Type
- Owned Capability
- Current State
- Responsibilities
- Related

## Recommended Fields

- Dependencies
- Related Components
- Related Tests
- Related Opportunities
- Related Learnings

## Optional Fields

- Consumers
- APIs
- Risks
- Verification Notes

## Validation Rules

### V1

Every Engineering Component must possess a unique identifier.

### V2

Every Engineering Component must follow KTS.012.

### V3

Every Engineering Component must reference exactly one primary owning Capability.

### V4

Every Engineering Component must define at least one responsibility.

### V5

Every Engineering Component should maintain at least three meaningful relationships.

### V6

Mandatory fields must be present.

### V7

Recommended fields should be completed whenever sufficient information exists.

### V8

Optional fields may be omitted.

### V9

Engineering Components shall not duplicate Capability definitions.

Capabilities describe desired outcomes.

Engineering Components describe implementation realization.

### V10

Engineering Component identifiers shall use the CMP prefix and follow KTS.010 Knowledge Object Identifier Standard.

## Template

# CMP.xxx Component Name

## Purpose

## Component Type

## Owned Capability

## Current State

## Responsibilities

### R1

### R2

### R3

## Dependencies

## Related Components

## Related Tests

## Related Opportunities

## Related Learnings

## Consumers

## APIs

## Risks

## Verification Notes

## Related

## Related

[[KTS.000 Knowledge Standard]]

[[KTS.001 Capability Standard]]

[[KTS.010 Knowledge Object Identifier Standard]]

[[ADR.010 Knowledge Planning Precedes Engineering Execution]]