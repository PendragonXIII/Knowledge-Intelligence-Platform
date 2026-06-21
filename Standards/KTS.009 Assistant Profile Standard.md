# KTS.009 Assistant Profile Standard

## Purpose

Define the structure and governance requirements for Assistant Profiles.

Assistant Profiles govern how assistants consume knowledge, apply reasoning, load context, communicate information and visualize governance artifacts.

Assistant Profiles define assistant behavior.

---

## Standard Structure

Every Assistant Profile shall contain the following sections.

### 1. Purpose

### 2. Reasoning Principles

### 3. Knowledge Consumption

### 4. Context Loading Behavior

### 5. Communication Style

### 6. Visualization Preferences

### 7. Session Behavior

### 8. Execution Model

Define how the assistant executes governed activities and interacts with Playbooks.

### 9. Decision Support Behavior

Define how the assistant supports prioritization, recommendations and decision-making.

### 10. Governance Alignment

### 11. Related

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
- Execution Model
- Decision Support Behavior
- Governance Alignment

---

## Recommended Fields

- Preferred Audience
- Decision Support Style
- Escalation Behavior
- Clarification Strategy
- Capability Presentation Preferences
- Roadmap Presentation Preferences
- Engineering Handoff Behavior
- Playbook Interaction

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

### V7

Assistant Profiles must define assistant-specific behavior and must not merely duplicate other Assistant Profiles.

### V8

Assistant Profiles shall define how governed activities interact with Playbooks when applicable.

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

## Execution Model

...

## Decision Support Behavior

...

## Governance Alignment

...

## Related

...

---

## Related

[[KTS.000 Knowledge Standard]]

[[PLB.000 Knowledge Session Initialization]]

[[LRN.015 Playbook-Driven Execution]]