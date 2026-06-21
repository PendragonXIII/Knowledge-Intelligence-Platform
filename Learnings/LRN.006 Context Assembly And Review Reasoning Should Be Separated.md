# LRN.006 Context Assembly And Review Reasoning Should Be Separated

## Standard

[[KTS.002 Learning Standard]]

## Learning

Knowledge review systems should separate context assembly from reasoning.

Python services should focus on:

- retrieval
- relationship discovery
- reference validation
- context assembly

Experience showed that Large Language Models are better suited for:

- governance review
- inconsistency detection
- recommendation generation
- relationship recommendations
- maintenance analysis

The purpose of the backend is to provide evidence-rich context, not to duplicate reasoning capabilities already available in the LLM.

## Evidence

Multiple review-oriented services were implemented before recognizing that the primary value comes from supplying structured context to the LLM.

The resulting architecture became simpler and more aligned with the strengths of each component.

## Impact

Improves:

- maintainability
- flexibility
- development speed
- AI effectiveness

## Related

[[EID.03 Context Intelligence]]

[[EID.04 Governance Intelligence]]

[[EID.07 Validation Intelligence]]

[[EID.08 Knowledge Intelligence]]

[[OP.014 Knowledge Validation Service]]

[[OP.017 Review Context Automation]]