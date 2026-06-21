# LRN.005 GitHub-Based Repository Access Improves Deployment Portability

## Standard

[[KTS.002 Learning Standard]]

## Learning

Knowledge Intelligence Services should treat the GitHub Knowledge Repository as the authoritative source of truth.

Repository access should not depend on:

- local file systems
- local development environments
- machine-specific paths
- synchronized folders

Knowledge retrieval and repository maintenance services should operate against GitHub APIs to ensure consistent behavior across:

- local development
- Railway deployments
- GPT Actions
- future AI agents

## Evidence

During end-to-end validation, the system successfully executed GPT Actions and Railway endpoints but failed because retrieval services depended on a local Windows path.

The issue was resolved by replacing local repository access with GitHub-backed retrieval services.

## Impact

Improves:

- deployment portability
- agent interoperability
- repository consistency
- production reliability

## Related

[[EID.01 Repository Intelligence]]

[[EID.03 Context Intelligence]]

[[EID.08 Knowledge Intelligence]]

[[CNS.006 Git-Managed Knowledge Repository]]

[[OP.012 Knowledge Retrieval Service]]