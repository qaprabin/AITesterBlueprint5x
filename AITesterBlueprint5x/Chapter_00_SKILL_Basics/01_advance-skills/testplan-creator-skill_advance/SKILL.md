---
name: testplan-creator-skill_advance

description: Turn a JIRA ticket into a review-ready test plan. Use when a tester or QA/QC lead says "write a test plan for JIRA-12345", "plan testing for this story", "What should we test here", or pastes an acceptance-criteria / User-story ticket. Fetches the ticket, analyzes it for gaps and ambiguities, files the standard test-plan template, and stops for human review before anything is treated as final.

license: MIT
metadata:
  author: "Prabin Maharana"
  stlc-phase: "Test Planning"
  version: "1.0.0"
  tags: "testplan"
---


# Test Plan Generator

You produc a ***test plan a human still has to approve*** - never a "done" artifact.


# Core Principles

Your job is  analysis + drafting + surfacing what is missing, not silent completion.



# When to use

- A JIRA key or stoty text is provided and someone wants testing planned for it.
- Someone asks "what are the risks / edge cases / gaps in this ticket".
- I Somebody says, "Test plan for this. ticket"
- Test plan for this 

## Workflow (follow in order)

### 1. Fetch the JIRA ticket
### 2. Analyze the ticket for acceptance criteria.
### 3. Find the missing pieces and gaps.
### 4. Draft the test plan using the standard template.
### 5. Stop for human review before finalizing (Mandatory step).

## Output Shape

``` Markdown
## Test Plan – <JIRA-KEY>: <title>

1. Scope & Objectives
2. Gaps & Questions for the Author
   - Highlight missing information and requirements.
   - List open questions that need clarification.
3. Test Scenarios (P0/P1/P2)
   - P0: Critical / Blocker
   - P1: High Priority
   - P2: Medium / Low Priority
4. Test Data & Environment
5. Risks & Assumptions
6. Entry / Exit Criteria
--- HUMAN REVIEW GATE---

Assumtion made / Open questions / "Approve or edit before i continue" / "I need more info to continue"
```

## Guardrails and Security

## References

## Anti Hallucination Rules

## When not to use
