# LRN.007 Explicit API Schemas Improve GPT Interoperability

## Standard

[[KTS.002 Learning Standard]]

## Learning

GPT Actions depend heavily on the quality of OpenAPI schema definitions.

Endpoints should expose explicit request models with clearly defined properties.

Generic dictionary-based request bodies reduce GPT’s ability to:

- understand available fields
- construct valid requests
- execute actions reliably

Explicit request models improve GPT interoperability and action reliability.

## Evidence

Repository write endpoints existed and functioned correctly but generated GPT import warnings because request schemas lacked explicit properties.

Introducing dedicated request models removed schema errors and improved GPT action compatibility.

## Impact

Improves:

- GPT usability
- action reliability
- API clarity
- integration quality

## Related

[[EID.01 Repository Intelligence]]

[[EID.03 Context Intelligence]]

[[EID.08 Knowledge Intelligence]]

[[EID.09 Knowledge Intelligence Services]]

[[LRN.006 Context Assembly And Review Reasoning Should Be Separated]]