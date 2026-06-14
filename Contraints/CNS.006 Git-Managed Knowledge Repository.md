## Status

Active

## Constraint

The Knowledge Layer shall be maintained as a Git-managed repository.

## Rationale

Git provides:

- version control
- change traceability
- rollback capability
- branch-based experimentation
- repository portability
- AI-accessible storage

The Knowledge Layer must remain usable without requiring proprietary synchronization services.

## Applicable Knowledge Objects

- Capabilities
- Opportunities
- Constraints
- Learnings
- ADRs
- Playbooks
- Roadmaps
- Knowledge Template Standards

## Requirements

### R1 – Git Repository

All knowledge objects shall be stored within a Git-managed repository.

### R2 – Markdown Format

Knowledge objects shall be stored as Markdown files.

### R3 – Offline Operation

The Knowledge Layer shall remain fully usable when operating offline.

### R4 – Obsidian Compatibility

The repository structure shall remain compatible with Obsidian.

### R5 – Repository Portability

Knowledge objects shall remain portable across platforms and tooling.

### R6 – Version Traceability

Changes to knowledge objects shall be traceable through Git history.

### R7 – Vendor Independence

Knowledge Layer operation shall not depend on proprietary synchronization services.

### R8 – Synchronization Separation

Synchronization mechanisms shall remain separate from governance and knowledge structures.

### R9 – Windows Compatibility

Knowledge object identifiers shall not use reserved Windows device names.

Examples include:

- CON
- PRN
- AUX
- NUL
- COM1-COM9
- LPT1-LPT9

## Implications

Git becomes the system of record for the Knowledge Layer.

Obsidian becomes the primary authoring interface.

OneDrive may be used as a synchronization mechanism but is not the authoritative source.

Knowledge Intelligence capabilities must operate against repository-managed knowledge objects.

Constraint identifiers use the prefix CNS instead of CON to ensure compatibility with Windows and OneDrive synchronization.

## Related

[[CNS.005 Knowledge Object Standards]]

[[PLB.003 Knowledge Object Creation]]

[[ADR.002 Obsidian as Knowledge Authoring Layer]]

[[EID.08 Knowledge Intelligence]]