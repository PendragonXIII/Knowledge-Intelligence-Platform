# KTS.009 Assistant Profile Standard

## Purpose

Define the structure and governance requirements for Assistant Profiles.

Assistant Profiles govern how assistants consume knowledge, apply reasoning, load context, communicate information and visualize governance artifacts.

Assistant Profiles do not define domain knowledge.

Assistant Profiles define assistant behavior.

---

## Standard Structure

Every Assistant Profile shall contain the following sections.

### 1. Purpose

Describe the role and primary objective of the assistant.

### 2. Reasoning Principles

Define how the assistant approaches analysis, synthesis, evaluation and recommendation generation.

### 3. Knowledge Consumption

Define how the assistant prioritizes and consumes available knowledge sources.

### 4. Context Loading Behavior

Define how the assistant retrieves and expands context.

### 5. Communication Style

Define communication principles and audience expectations.

### 6. Visualization Preferences

Define how governance artifacts, maturity models, priorities and capability information should be presented.

### 7. Session Behavior

Define expected behavior during session initialization, context discovery and session execution.

### 8. Governance Alignment

Define how the assistant aligns with standards, playbooks and governance artifacts.

### 9. Related

Define related standards, playbooks and governance references.

---

## Mandatory Fields

Every Assistant Profile must define:

- ID
- Name
- Purpose
- Reasoning Principles
- Knowledge Consumption
- Context Loading Behavior
- Communication Style
- Visualization Preferences
- Session Behavior
- Governance Alignment

---

## Recommended Fields

Where applicable:

- Preferred Audience
- Decision Support Style
- Escalation Behavior
- Clarification Strategy
- Capability Presentation Preferences
- Roadmap Presentation Preferences

---

## Optional Fields

- Examples
- Anti-Patterns
- Assistant-Specific Guidance

---

## Validation Rules

### V1

Every Assistant Profile must possess a unique identifier.

### V2

Every Assistant Profile must follow KTS.009.

### V3

Every Assistant Profile must define all mandatory fields.

### V4

Assistant Profiles must govern behavior and presentation rather than domain knowledge.

### V5

Assistant Profiles must remain compatible with PLB.000 Knowledge Session Initialization.

### V6

Assistant Profiles may influence visualization and communication but must not redefine governance semantics defined elsewhere.

---

## Template

# ASP.xxx Assistant Profile

## Purpose

...

## Reasoning Principles

...

## Knowledge Consumption

...

## Context Loading Behavior

...

## Communication Style

...

## Visualization Preferences

...

## Session Behavior

...

## Governance Alignment

...

## Related

...

---

## Related

[[KTS.000 Knowledge Standard]]

[[PLB.000 Knowledge Session Initialization]]