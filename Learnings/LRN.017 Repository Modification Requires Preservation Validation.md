# LRN.017 Repository Modification Requires Preservation Validation

## Observation

During governance updates, an existing Assistant Profile was unintentionally reduced because a modification operation replaced significant portions of the original content.

The issue was only detected through manual review.

## Learning

Modifying an existing repository artifact is fundamentally different from creating a new artifact.

Repository modifications require preservation validation.

## Required Validation Sequence

1. Read existing artifact.
2. Identify intended changes.
3. Identify content that must be preserved.
4. Apply modification.
5. Re-read artifact.
6. Validate preserved content remains present.
7. Commit only after successful validation.

## Anti-Pattern

Read
↓
Modify
↓
Write

without validating preservation.

## Preferred Pattern

Read
↓
Analyze
↓
Preservation Validation Plan
↓
Modify
↓
Re-Read
↓
Preservation Validation
↓
Commit

## Outcome

Repository modifications become safer, more traceable and less likely to introduce accidental governance regressions.

## Related

[[PLB.013 Knowledge Object Modification]]

[[PLB.010 Repository Consistency Review]]