# PLB.010 Repository Consistency Review

## Purpose

Provide a repeatable process for assessing the internal consistency, governance quality and structural integrity of the Knowledge Repository.

## Preconditions

- Repository access available
- Governing standards available
- Relevant ADRs available

## Process

### Step 1 – Repository Inventory

Identify:

- Object types
- Folder structure
- Identifier ranges
- Governance artifacts

### Step 2 – Identifier Validation

Validate:

- Unique identifiers
- Prefix compliance
- Missing identifiers
- Duplicate identifiers

### Step 3 – Governance Review

Review consistency between:

- Standards
- Playbooks
- ADRs
- Assistant Profiles

### Step 4 – Relationship Review

Identify:

- Missing references
- Broken references
- Orphaned objects
- Duplicate relationships

### Step 5 – Architectural Consistency

Validate alignment between:

- ADRs
- Standards
- Playbooks
- Capability structures

### Step 6 – Findings Classification

Classify findings as:

- DUPLICATE_IDENTIFIER
- GOVERNANCE_GAP
- GOVERNANCE_CONFLICT
- REFERENCE_GAP
- STRUCTURE_INCONSISTENCY
- ARCHITECTURE_MISMATCH

### Step 7 – Recommendations

Provide:

- Required corrections
- Recommended improvements
- Governance actions

## Success Criteria

The repository is:

- internally consistent
- uniquely identified
- governance-aligned
- traceable
- maintainable

## Related

[[KTS.010 Knowledge Object Identifier Standard]]

[[ADR.009 ADR Lifecycle and Resolution Strategy]]

[[PLB.004 Knowledge Governance Review]]