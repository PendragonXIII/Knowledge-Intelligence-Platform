## Status

Active

## Constraint

All knowledge objects must comply with approved Knowledge Template Standards (KTS).

## Rationale

Standardized structures improve:
- consistency    
- discoverability    
- maintainability    
- AI consumption    
- automated governance    
- context assembly    
- knowledge validation    
- knowledge generation    

## Applicable Knowledge Objects

- Capabilities    
- Opportunities    
- Constraints    
- Learnings    
- ADRs    
- Playbooks    
- Roadmaps    

## Requirements

### R1 – Unique Identifier

Every knowledge object must have a unique and stable identifier.

Examples:
- EID.08    
- OP.003    
- CNS.005    
- ADR.002    

### R2 – Approved Knowledge Standard

Every knowledge object must follow an approved Knowledge Template Standard (KTS).

### R2a – Standard Reference

Every knowledge object shall explicitly reference the Knowledge Template Standard used for its creation.

Examples:
- [[KTS.001 Capability Standard]]    
- [[KTS.002 Opportunity Standard]]    
- [[KTS.003 Constraint Standard]]    
- [[KTS.004 Learning Standard]]    
- [[KTS.005 ADR Standard]]    
- [[KTS.006 Playbook Standard]]    
- [[KTS.007 Roadmap Standard]]    

### R2b – Standard Governance

Knowledge Template Standards are governance artifacts and must be maintained and reviewed accordingly.
### R2c – Standard Compliance

All Knowledge Template Standards must comply with:
[[KTS.000 Knowledge Standard Standard]]

### R3 – Relationships

Every knowledge object should maintain at least three meaningful relationships to other knowledge objects.

### R4 – AI Consumability

Knowledge objects must remain structured, machine-readable and suitable for AI-assisted reasoning, validation and context assembly.

### R5 – Opportunity Assignment

Every Opportunity must be linked to at least one Capability.

### R6 – Capability Traceability

Every Capability must reference at least one related Opportunity.

### R7 – Roadmap Governance

Every Roadmap phase must define:
- Status    
- Objective    
- Exit Criteria    

### R8 – Standard Compliance

The presence of an approved Knowledge Template Standard is mandatory.

Complete population of all standard fields is recommended but not mandatory.

### R9 – Temporary Exceptions

Newly created knowledge objects may temporarily exist with fewer than three relationships.

Relationship requirements must be fulfilled before the next governance review.

### R10 – Governance Artifact Identification

Knowledge Template Standards and other governance artifacts must possess unique identifiers.

## Implications

Knowledge objects must use approved Knowledge Template Standards.

Knowledge objects must reference their governing standard.

Knowledge creation follows defined workflows.

Knowledge standards must be maintained as governance artifacts.

Knowledge governance can be reviewed systematically.

Knowledge validation can be automated.

AI systems can discover, generate and validate knowledge objects through standard references.

## Related

[[KTS.000 Knowledge Standard Standard]]

[[PLB.003 Knowledge Object Creation]]

[[CNS.004 Knowledge Must Remain AI Consumable]]

[[EID.08 Knowledge Intelligence]]