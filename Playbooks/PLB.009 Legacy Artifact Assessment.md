# PLB.009 Legacy Artifact Assessment

## Standard

[[KTS.006 Playbook Standard]]

## Purpose

Provide a governed process for assessing legacy engineering, architecture and governance artifacts against the Knowledge Repository.

## When to Use

Use this playbook when reviewing:

- legacy repositories
- architecture documents
- governance documents
- engineering documentation
- historical decisions
- exported AI conversations

## Process

### Step 1 – Initialize Context

Execute:

- [[PLB.000 Knowledge Session Initialization]]

Load relevant repository context before assessing legacy artifacts.

### Step 2 – Read Legacy Artifact

Identify:

- purpose
- scope
- decisions
- constraints
- capabilities
- learnings
- opportunities

### Step 3 – Extract Knowledge Candidates

Identify candidate:

- Capabilities
- Constraints
- Learnings
- Opportunities
- ADRs
- Roadmap Items
- Relationships

### Step 4 – Compare Against Repository

Determine whether identified knowledge:

- already exists
- partially exists
- conflicts with existing knowledge
- is missing from the repository

### Step 5 – Generate Findings

Classify findings as:

- New Knowledge Object
- Knowledge Object Update
- Relationship Update
- Governance Finding
- Repository Gap

### Step 6 – Recommend Repository Changes

Recommend:

- object creation
- object modification
- relationship creation
- governance updates
- roadmap updates

### Step 7 – Execute Governed Updates

Apply approved changes using:

- [[PLB.003 Knowledge Object Creation]]
- [[PLB.008 Knowledge Object Modification]]

## Expected Outputs

- Knowledge Candidates
- Repository Gap Analysis
- Governance Findings
- Relationship Recommendations
- Knowledge Object Recommendations

## Related

[[PLB.000 Knowledge Session Initialization]]

[[PLB.002 Session-to-Knowledge Extraction]]

[[PLB.006 Knowledge Object Assessment]]

[[PLB.007 Repository Consistency Review]]

[[PLB.008 Knowledge Object Modification]]

[[EID.10 Knowledge Extraction Intelligence]]

[[EID.11 Knowledge Comparison Intelligence]]