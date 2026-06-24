# OP.019 Assistant Profile Bootstrap Alignment

## Purpose

Ensure every dedicated assistant is explicitly aligned to its corresponding Assistant Profile through bootstrap instructions.

## Problem

Assistant Profiles exist within repository governance but may not be explicitly activated by assistant-specific bootstrap instructions.

This can lead to behavioral bleedover between assistant types and reduce governance consistency.

## Opportunity

Review each dedicated assistant and explicitly align bootstrap instructions with the intended Assistant Profile.

Examples:

- Knowledge Assistant → ASP.001
- Engineering Assistant → ASP.002
- Garden Assistant → ASP.003

Future Assistant Profiles should be evaluated as part of assistant creation.

## Expected Benefits

- Clear assistant mode selection
- Reduced cross-domain behavior bleedover
- Improved governance compliance
- More predictable context loading behavior

## Status

Proposed

## Related

[[ASP.001 Knowledge Assistant Profile]]

[[ASP.002 Engineering Assistant Profile]]

[[ASP.003 Garden Assistant Profile]]

[[PLB.000 Knowledge Session Initialization]]