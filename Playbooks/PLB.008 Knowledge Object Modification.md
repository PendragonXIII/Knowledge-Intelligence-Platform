## Purpose

Provide a governed process for modifying existing Knowledge Objects while preventing accidental loss of content, relationships or governance information.

## Preconditions

- Target object exists
- Governing standard exists
- Modification objective is defined

## Process

### Step 1 – Read Existing Object

Load the current object.

Record:

- line count
- optional character count
- optional section count

### Step 2 – Identify Intended Change

Explicitly document:

- sections to add
- sections to modify
- sections to remove

### Step 3 – Preservation Assessment

Identify content that must remain unchanged.

Examples:

- governance sections
- relationships
- historical context
- validation rules
- architecture rationale

### Step 4 – Planned Change Validation

Before writing, calculate:

- projected line count
- projected delta
- expected preservation impact

If the projected delta is inconsistent with the intended change, stop and review before continuing.

### Step 5 – Apply Modification

Apply only the intended changes.

### Step 6 – Re-Read Object

Load the updated object when repository consistency permits.

### Step 7 – Preservation Validation

Verify:

- intended changes exist
- preserved sections remain present
- relationships remain present
- governance content remains present

### Step 8 – Delta Validation

Compare:

- original line count
- planned line count
- actual line count when available

Report the delta as part of the modification outcome.

Significant unexpected variance requires review before completion.

### Step 9 – Consistency Validation

Validate alignment with:

- governing standards
- related ADRs
- related Playbooks
- related Learnings

### Step 10 – Commit

Commit only after successful preservation validation.

## Anti-Pattern

Read
↓
Modify
↓
Write

without preservation validation.

Read
↓
Large unexplained delta
↓
Write

without delta assessment.

## Success Criteria

The modified object:

- contains intended changes
- preserves existing knowledge
- remains governance compliant
- remains internally consistent
- includes modification delta assessment

## Related

[[LRN.017 Repository Modification Requires Preservation Validation]]

[[PLB.003 Knowledge Object Creation]]

[[PLB.007 Repository Consistency Review]]