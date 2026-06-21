## Purpose

Define the structure and governance requirements for Knowledge Template Standards (KTS).

## Standard Structure

Every Knowledge Template Standard shall contain the following sections.

### 1. Purpose

Describe the intent of the knowledge object type.

### 2. Mandatory Fields

Define fields that must be present.

### 3. Recommended Fields

Define fields that should be completed whenever sufficient information exists.

### 4. Optional Fields

Define fields that may be omitted.

### 5. Validation Rules

Define validation requirements for the knowledge object type.

### 6. Template

Define the canonical structure of the knowledge object.

### 7. Related

Define governance and capability references.

## Validation Rules

### V1

Every KTS document must possess a unique identifier.

### V2

Every KTS document must follow KTS.000.

### V3

Every KTS document must define Mandatory, Recommended and Optional fields.

### V4

Every KTS document must define Validation Rules.

### V5

Every KTS document must provide a canonical template.

### V6

Every governed Knowledge Object Type should be defined by a corresponding KTS standard.

### V7

Assistant Profiles are valid Knowledge Objects and shall follow KTS.009 Assistant Profile Standard.

### V8

Governed activities should be executed through their corresponding Playbooks whenever available.

Before execution:

1. Identify activity type.
2. Identify governing Playbook.
3. Load Playbook.
4. Execute activity.

### V9

Knowledge Object lifecycle activities shall use the appropriate Playbook.

- Create Knowledge Object → PLB.003 Knowledge Object Creation
- Modify Knowledge Object → PLB.013 Knowledge Object Modification

## Related

[[KTS.009 Assistant Profile Standard]]

[[KTS.010 Knowledge Object Identifier Standard]]

[[LRN.015 Playbook-Driven Execution]]

[[CNS.005 Knowledge Object Standards]]

[[PLB.000 Knowledge Session Initialization]]

[[PLB.003 Knowledge Object Creation]]

[[PLB.013 Knowledge Object Modification]]

[[EID.08 Knowledge Intelligence]]