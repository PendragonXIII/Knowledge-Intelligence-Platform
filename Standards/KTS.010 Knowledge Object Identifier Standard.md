# KTS.010 Knowledge Object Identifier Standard

## Purpose

Define identifier allocation, naming conventions and validation requirements for Knowledge Objects.

---

## Mandatory Rules

### ID Uniqueness

Every Knowledge Object must possess a unique identifier.

### Sequential Allocation

New identifiers shall be allocated using the next available identifier within the corresponding object type.

### Validation Before Creation

Before creating a new Knowledge Object:

1. Load existing objects of the same type.
2. Determine the highest existing identifier.
3. Allocate the next available identifier.
4. Validate naming conventions.

---

## Identifier Prefixes

### Learnings

LRN.xxx

### Opportunities

OP.xxx

### Constraints

CNS.xxx

### Assistant Profiles

ASP.xxx

### Knowledge Template Standards

KTS.xxx

### Playbooks

PLB.xxx

---

## Validation Rules

### V1

Identifiers must be unique.

### V2

Identifiers must follow the approved prefix convention.

### V3

Identifiers must be validated before object creation.

### V4

Object type and identifier prefix must match.

---

## Related

[[KTS.000 Knowledge Standard]]

[[PLB.003 Knowledge Object Creation]]

[[LRN.014 Repository Object Creation Requires ID Validation]]