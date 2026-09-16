
# Content Governance

## Purpose

Use this file to determine:

- where new BPR Ringmaster content belongs
- which file owns each major topic
- how to avoid duplication
- how to resolve conflicts
- when to create a new file

The objective is to maintain one clear source of truth for each major behavior.

## Core Principle

One rule should have one owner.

Other files may:

- reference it
- summarize it
- apply it
- test it
- provide examples of it

They should not independently redefine it.

---

# Repository Responsibilities

## Root Files

Root files control overall GPT behavior and major operating modes.

Current root files include:

- README.md
- LICENSE
- GPT_INSTRUCTIONS.md
- PROMPT_STARTERS.md
- PRACTICE_MODE_INSTRUCTIONS.md
- COACH_MODE_INSTRUCTIONS.md

## Knowledge Folder

Knowledge files own what the caller should know, say, and do.

Examples:

- positioning
- call flow
- call openings
- objection handling
- scheduling
- email follow-up
- role identification
- recovery

## Simulation Folder

Simulation files own how the simulated prospect and practice environment behave.

Examples:

- prospect behavior
- difficulty
- scenarios
- hidden variables
- objections raised
- interruptions
- realism
- startup
- simulation ending

## Coaching Folder

Coaching files own how caller performance is evaluated, explained, and improved.

Examples:

- scoring
- feedback
- metrics
- common mistakes
- retry drills
- skill development
- progress tracking

## Reference Folder

Reference files provide fast lookup and decision support.

Examples:

- approved language
- language to avoid
- facts requiring confirmation
- variables
- meeting-type matrix
- objection matrix
- role matrix
- verification guidance

Reference files should not replace full Knowledge guidance.

## Maintenance Folder

Maintenance files govern:

- testing
- regression checking
- repository organization
- user operating guidance

Maintenance files should not introduce new call policy, new prospect behavior, or new scoring rules.

---

# Source of Truth by Topic

## Overall GPT Identity and Behavior

Owner:

- GPT_INSTRUCTIONS.md

## Practice Mode

Owner:

- PRACTICE_MODE_INSTRUCTIONS.md

## Coach Mode

Owner:

- COACH_MODE_INSTRUCTIONS.md

## Prompt Starters

Owner:

- PROMPT_STARTERS.md

Prompt starters provide entry points only.

They do not define underlying behavior.

---

# Knowledge Ownership

## Core Positioning

Owner:

- knowledge/01_CORE_POSITIONING.md

## Call Objectives

Owner:

- knowledge/02_CALL_OBJECTIVES.md

## Master Call Flow

Owner:

- knowledge/03_MASTER_CALL_FLOW.md

## Call Openings

Owner:

- knowledge/04_CALL_OPENINGS.md

## Analyst and Research-Team Positioning

Owner:

- knowledge/05_ANALYST_PROJECT_FRAME.md

## 15-to-20-Minute Overview

Owner:

- knowledge/06_15_MINUTE_OVERVIEW.md

## 60-Minute Analyst Briefing

Owner:

- knowledge/07_60_MINUTE_BRIEFING.md

## Gatekeeper Caller Strategy

Owner:

- knowledge/08_GATEKEEPER_PLAYBOOK.md

## Persona Messaging

Owner:

- knowledge/09_PERSONAS.md

## Objection Handling

Owner:

- knowledge/10_OBJECTION_HANDLING.md

## Soft-No Recovery

Owner:

- knowledge/11_SOFT_NO_RECOVERY.md

## FAQ

Owner:

- knowledge/12_FAQ.md

## RAIN Framework

Owner:

- knowledge/13_RAIN_FRAMEWORK.md

This is an internal design framework.

It should not override actual call flow or approved language.

## Call Gates

Owner:

- knowledge/14_CALL_GATES.md

## Permission and Microcommitments

Owner:

- knowledge/15_PERMISSION_MICROCOMMITMENTS.md

## Scheduling

Owner:

- knowledge/16_SCHEDULING.md

## Voicemail

Owner:

- knowledge/17_VOICEMAIL.md

## Timing and Trigger Events

Owner:

- knowledge/18_TIMING_TRIGGER_EVENTS.md

## Tone and Delivery

Owner:

- knowledge/19_TONE_DELIVERY.md

## Accuracy Guardrails

Owner:

- knowledge/20_ACCURACY_GUARDRAILS.md

## Commercial Versus Research

Owner:

- knowledge/21_COMMERCIAL_VS_RESEARCH.md

## Email Follow-Up

Owner:

- knowledge/22_EMAIL_FOLLOWUP.md

## Scenario-Specific Caller Strategy

Owner:

- knowledge/23_CALL_SCENARIO_BRANCHES.md

## Role Identification

Owner:

- knowledge/24_ROLE_IDENTIFICATION.md

## Previous Recipient Path

Owner:

- knowledge/25_PREVIOUS_RECIPIENT_PATH.md

## Conversation Branches

Owner:

- knowledge/26_CONVERSATION_BRANCHES.md

## Call Recovery

Owner:

- knowledge/27_CALL_RECOVERY.md

---

# Simulation Ownership

## Simulation Engine

Owner:

- simulation/01_SIMULATION_ENGINE.md

## Difficulty Levels

Owner:

- simulation/02_DIFFICULTY_LEVELS.md

## Prospect Behaviors

Owner:

- simulation/03_PROSPECT_BEHAVIORS.md

## Scenario Library

Owner:

- simulation/04_SCENARIO_LIBRARY.md

## Objection Selection

Owner:

- simulation/05_OBJECTION_RANDOMIZER.md

## Simulation Outcomes

Owner:

- simulation/06_CALL_OUTCOMES.md

## Email Follow-Up Simulation

Owner:

- simulation/07_EMAIL_FOLLOWUP_SIMULATION.md

## Hidden Variables

Owner:

- simulation/08_HIDDEN_SCENARIO_VARIABLES.md

## Interruptions and Curveballs

Owner:

- simulation/09_INTERRUPTIONS_AND_CURVEBALLS.md

## Gatekeeper Simulation Behavior

Owner:

- simulation/10_GATEKEEPER_SCENARIOS.md

## Multi-Person Calls

Owner:

- simulation/11_MULTI_PERSON_CALLS.md

## Simulation Realism

Owner:

- simulation/12_REALISM_RULES.md

## Simulation Startup and Disclosure

Owner:

- simulation/13_SIMULATION_STARTUP_AND_DISCLOSURE.md

## Simulation Ending and Coaching Handoff

Owner:

- simulation/14_SIMULATION_END_AND_HANDOFF.md

---

# Coaching Ownership

## What Is Scored

Owner:

- coaching/01_SCORECARD.md

## What Scores Mean

Owner:

- coaching/02_SCORING_RUBRIC.md

## Feedback Structure

Owner:

- coaching/03_FEEDBACK_FRAMEWORK.md

## Performance Metrics

Owner:

- coaching/04_CALL_METRICS.md

## Coaching Examples

Owner:

- coaching/05_COACHING_EXAMPLES.md

Examples do not override rules.

## Call Review Diagnostic

Owner:

- coaching/06_CALL_REVIEW_CHECKLIST.md

## Common Caller Mistakes

Owner:

- coaching/07_COMMON_CALLER_MISTAKES.md

## Retry Drills

Owner:

- coaching/08_RETRY_DRILLS.md

## Coaching by Skill

Owner:

- coaching/09_COACHING_BY_SKILL.md

## Progress Tracking

Owner:

- coaching/10_PROGRESS_TRACKING.md

---

# Reference Ownership

## Approved Language

Owner:

- reference/LANGUAGE_TO_USE.md

## Language to Avoid

Owner:

- reference/LANGUAGE_TO_AVOID.md

## Facts Requiring Confirmation

Owner:

- reference/FACTS_REQUIRING_CONFIRMATION.md

## Variables

Owner:

- reference/VARIABLES.md

## Meeting-Type Quick Reference

Owner:

- reference/MEETING_TYPE_MATRIX.md

This file summarizes meeting-selection guidance.

It does not redefine:

- knowledge/06_15_MINUTE_OVERVIEW.md
- knowledge/07_60_MINUTE_BRIEFING.md
- knowledge/16_SCHEDULING.md

## Objection Quick Reference

Owner:

- reference/OBJECTION_RESPONSE_MATRIX.md

This file summarizes objection direction.

It does not replace:

- knowledge/10_OBJECTION_HANDLING.md
- knowledge/11_SOFT_NO_RECOVERY.md
- knowledge/12_FAQ.md

## Role Quick Reference

Owner:

- reference/ROLE_MESSAGE_MATRIX.md

This file summarizes role-based relevance.

It does not replace:

- knowledge/09_PERSONAS.md
- knowledge/24_ROLE_IDENTIFICATION.md

## Escalation and Verification

Owner:

- reference/ESCALATION_AND_VERIFICATION_RULES.md

This file assists with verification decisions.

It does not override:

- knowledge/20_ACCURACY_GUARDRAILS.md
- knowledge/21_COMMERCIAL_VS_RESEARCH.md
- reference/FACTS_REQUIRING_CONFIRMATION.md

---

# Maintenance Ownership

## GPT Behavior Testing

Owner:

- maintenance/01_TESTING_CHECKLIST.md

## Repeatable Regression Tests

Owner:

- maintenance/02_REGRESSION_TESTS.md

## Repository Governance

Owner:

- maintenance/03_CONTENT_GOVERNANCE.md

## Team User Instructions

Owner:

- maintenance/04_USER_GUIDE.md

---

# Where New Content Goes

## New Approved Caller Wording

Update:

- reference/LANGUAGE_TO_USE.md

If the wording changes a broader framework, also update the Knowledge file that owns the behavior.

---

## New Language to Avoid

Update:

- reference/LANGUAGE_TO_AVOID.md

---

## New Objection

Primary update:

- knowledge/10_OBJECTION_HANDLING.md

Then, where relevant, update:

- reference/OBJECTION_RESPONSE_MATRIX.md
- simulation/05_OBJECTION_RANDOMIZER.md
- coaching/09_COACHING_BY_SKILL.md

Do not create a separate file for one objection.

---

## New Soft-No Pattern

Update:

- knowledge/11_SOFT_NO_RECOVERY.md

If it should appear in practice:

- simulation/05_OBJECTION_RANDOMIZER.md

---

## New FAQ

Update:

- knowledge/12_FAQ.md

If the answer contains a fact requiring confirmation:

- reference/FACTS_REQUIRING_CONFIRMATION.md

---

## New Scheduling Rule

Update:

- knowledge/16_SCHEDULING.md

If it changes the meeting-selection summary:

- reference/MEETING_TYPE_MATRIX.md

---

## New Microsoft Bookings Language

For call scheduling:

- knowledge/16_SCHEDULING.md

For email use:

- knowledge/22_EMAIL_FOLLOWUP.md

For approved wording:

- reference/LANGUAGE_TO_USE.md

---

## New Email Template

Update:

- knowledge/22_EMAIL_FOLLOWUP.md

Do not create a separate email-template file unless the existing file becomes unmanageable.

---

## New Persona Messaging

Update:

- knowledge/09_PERSONAS.md

---

## New Job Role

Update:

- knowledge/24_ROLE_IDENTIFICATION.md

If useful as a quick reference:

- reference/ROLE_MESSAGE_MATRIX.md

---

## New Scenario

Update:

- simulation/04_SCENARIO_LIBRARY.md

Do not place new practice scenarios in Maintenance.

---

## New Prospect Behavior

Update:

- simulation/03_PROSPECT_BEHAVIORS.md

---

## New Objection for Simulation

Update:

- simulation/05_OBJECTION_RANDOMIZER.md

The caller response itself still belongs in:

- knowledge/10_OBJECTION_HANDLING.md

---

## New Curveball

Update:

- simulation/09_INTERRUPTIONS_AND_CURVEBALLS.md

---

## New Gatekeeper Simulation Behavior

Update:

- simulation/10_GATEKEEPER_SCENARIOS.md

The caller's gatekeeper strategy belongs in:

- knowledge/08_GATEKEEPER_PLAYBOOK.md

---

## New Multi-Person Scenario

Update:

- simulation/11_MULTI_PERSON_CALLS.md

---

## New Hidden Variable

Update:

- simulation/08_HIDDEN_SCENARIO_VARIABLES.md

---

## New Realism Rule

Update:

- simulation/12_REALISM_RULES.md

Do not duplicate it in scenario files unless an example is needed.

---

## New Coaching Skill

Update:

- coaching/09_COACHING_BY_SKILL.md

---

## New Common Caller Mistake

Update:

- coaching/07_COMMON_CALLER_MISTAKES.md

---

## New Retry Drill

Update:

- coaching/08_RETRY_DRILLS.md

---

## New Metric

Update:

- coaching/04_CALL_METRICS.md

---

## New Scoring Rule

If it changes what is evaluated:

- coaching/01_SCORECARD.md

If it changes what a score means:

- coaching/02_SCORING_RUBRIC.md

Do not create scoring rules in Maintenance.

---

## New Fact Requiring Confirmation

Update:

- reference/FACTS_REQUIRING_CONFIRMATION.md

---

## New Variable

Update:

- reference/VARIABLES.md

Never invent the value of a missing variable.

---

## New Verification Rule

Update:

- reference/ESCALATION_AND_VERIFICATION_RULES.md

If it changes overall accuracy behavior, also review:

- knowledge/20_ACCURACY_GUARDRAILS.md

---

# Duplication Rule

Examples may appear in multiple files when they help explain how a rule is applied.

Rules should not be independently redefined.

Example:

The wording:

"[COMPANY] came to our attention during [ANALYST_NAME]'s research..."

may appear in several examples.

That is acceptable.

The underlying analyst-positioning rule should still be owned by:

- knowledge/05_ANALYST_PROJECT_FRAME.md

---

# Conflict Rule

If two files conflict:

1. identify which file owns the topic
2. follow the source-of-truth file
3. update the secondary file so it no longer conflicts
4. do not create a third workaround file

---

# Hierarchy for Conflict Resolution

Use this general order:

1. GPT_INSTRUCTIONS.md
2. PRACTICE_MODE_INSTRUCTIONS.md or COACH_MODE_INSTRUCTIONS.md when that mode is active
3. Knowledge source-of-truth file
4. Simulation or Coaching source-of-truth file for its own domain
5. Reference quick-reference file
6. Maintenance testing or user-guide material
7. examples

A lower-level example should never override a higher-level rule.

---

# File Creation Rule

Create a new file only when:

- the topic has a distinct function
- existing files do not already own the topic
- the content is substantial enough to warrant separation
- the new file improves maintainability
- it will not create another source of truth

Before creating a new file, ask:

"Can this be added to the existing owner instead?"

If yes, update the existing file.

---

# Testing After Changes

After modifying a source-of-truth file:

1. identify the relevant tests in maintenance/01_TESTING_CHECKLIST.md
2. run appropriate tests from maintenance/02_REGRESSION_TESTS.md
3. check related quick-reference files for stale summaries
4. update examples only where necessary
5. avoid editing unrelated files

---

# Final Governance Principle

Keep the repository simple:

Root
= controls the GPT

Knowledge
= teaches the caller

Simulation
= controls the prospect

Coaching
= evaluates and improves the caller

Reference
= provides fast lookup and guardrails

Maintenance
= tests and governs the system

One rule should have one owner.
