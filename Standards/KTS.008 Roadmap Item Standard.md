## Purpose

Define the standard structure and governance requirements for Roadmap Item knowledge objects.

Roadmap Items represent discrete initiatives, work packages or milestones that contribute to the delivery of a Roadmap.

## Mandatory Fields

- Roadmap
- Objective
- Status
- Related

## Recommended Fields

- Sources
- Scope
- Success Criteria
- Priority

## Optional Fields

- Dependencies
- Risks
- Assumptions
- Notes

## Validation Rules

### V1

Every Roadmap Item must have a unique identifier.

### V2

Every Roadmap Item must follow KTS.008.

### V3

Every Roadmap Item must reference a parent Roadmap.

### V4

Every Roadmap Item must define a clear objective.

### V5

Every Roadmap Item must define a status.

### V6

Every Roadmap Item should maintain at least three meaningful relationships.

### V7

Mandatory fields must be present.

### V8

Recommended fields should be completed whenever sufficient information exists.

### V9

Optional fields may be omitted.

## Template

# RMI.xxx Roadmap Item Name

## Standard

[[KTS.008 Roadmap Item Standard]]

## Roadmap

[[RMP.xxx Roadmap Name]]

## Objective

## Sources

## Scope

## Success Criteria

## Priority

## Status

## Dependencies

## Risks

## Assumptions

## Notes

## Related

## Related

[[KTS.000 Knowledge Standard]]

[[KTS.007 Roadmap Standard]]

[[CNS.005 Knowledge Object Standards]]

[[PLB.003 Knowledge Object Creation]]

[[EID.08 Knowledge Intelligence]]