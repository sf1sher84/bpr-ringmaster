
# Testing Checklist

## Purpose

Use this checklist to verify that BPR Ringmaster is behaving correctly after changes to instructions, Knowledge, Simulation, Coaching, Reference, or Maintenance files.

This checklist tests the GPT itself.

It does not evaluate the caller's performance.

For caller-performance evaluation, use:

- coaching/01_SCORECARD.md
- coaching/02_SCORING_RUBRIC.md
- coaching/03_FEEDBACK_FRAMEWORK.md
- coaching/06_CALL_REVIEW_CHECKLIST.md

## Core Rule

Test behavior against the current source-of-truth files.

If a test fails, update the file that owns the behavior rather than creating a second rule somewhere else.

For file ownership, use:

- maintenance/03_CONTENT_GOVERNANCE.md

---

## 1. Core Positioning

Confirm that BPR Ringmaster:

- positions the outreach as research-led
- does not position the call as traditional sales outreach
- uses the named analyst when one is confirmed
- positions the caller as part of the research team supporting the analyst's work
- explains that the company surfaced during relevant industry research
- distinguishes nomination for evaluation from final recognition
- avoids overly promotional award language

Pass condition:

The outreach sounds research-led, credible, concise, and non-promotional.

---

## 2. Call Opening

Confirm that the opening:

- identifies the caller
- identifies Frost & Sullivan
- introduces the analyst or research context appropriately
- sounds conversational rather than scripted
- can include "How are you doing today?" naturally
- references a prior email when appropriate
- does not over-explain before creating dialogue

The opening should not sound apologetic or overly sales-oriented.

---

## 3. Familiarity Branching

Test three prospect states:

- familiar with Frost & Sullivan
- somewhat familiar
- unfamiliar

Confirm that the amount of explanation changes appropriately.

The GPT should not give every prospect the same explanation.

---

## 4. Named Analyst Positioning

Confirm that BPR Ringmaster:

- uses only a confirmed or scenario-provided analyst name
- does not invent analyst involvement
- does not imply the analyst personally requested the call unless confirmed
- distinguishes the analyst's role from the caller's role
- does not invent analyst findings or conclusions

---

## 5. Research Team Positioning

Confirm that the caller is positioned consistently as:

- part of the research team
- supporting the analyst's work
- helping coordinate the conversation

The GPT should not imply that the caller is the lead analyst unless the scenario explicitly says so.

---

## 6. Best Practices Recognition Positioning

Confirm that the GPT:

- describes BPR as part of the research and evaluation process
- does not present nomination as final recognition
- does not imply the company has already won
- does not present the program primarily as an award sale
- does not invent criteria, categories, or outcomes

---

## 7. 15-to-20-Minute Overview

Test with a prospect who is unfamiliar with Frost & Sullivan or BPR.

Confirm that the GPT:

- recognizes the 15-to-20-minute overview as the typical next step
- explains the purpose clearly
- does not describe the call as a full analyst briefing
- does not unnecessarily ask for 60 minutes

The overview should generally cover:

- Frost & Sullivan context
- why the company surfaced
- Best Practices Recognition
- evaluation process
- questions
- next steps

For full guidance, use:

- knowledge/06_15_MINUTE_OVERVIEW.md

---

## 8. 60-Minute Analyst Briefing

Test with:

- a contact who has already completed the overview
- a highly familiar contact
- a previous participant
- a previous recognition recipient

Confirm that the GPT:

- recognizes when a deeper briefing may be appropriate
- does not automatically require one simply because the contact is senior
- does not automatically require one simply because the company participated previously
- keeps the briefing focused on substantive company and market discussion

Possible discussion areas may include:

- strategy
- innovation
- growth
- customer value
- differentiation
- market leadership
- relevant evaluation areas

For full guidance, use:

- knowledge/07_60_MINUTE_BRIEFING.md
- knowledge/25_PREVIOUS_RECIPIENT_PATH.md

---

## 9. Gatekeeper Behavior

Test with a gatekeeper who asks:

"What is this regarding?"

Confirm that the GPT:

- gives concise research context
- identifies the analyst when confirmed
- explains the reason for the outreach accurately
- does not imply the executive is expecting the call
- seeks the right person, routing path, or scheduling process
- treats the gatekeeper respectfully

For full guidance, use:

- knowledge/08_GATEKEEPER_PLAYBOOK.md
- simulation/10_GATEKEEPER_SCENARIOS.md

---

## 10. Gatekeeper Expecting-the-Call Question

Test:

"Is she expecting your call?"

Confirm that BPR Ringmaster does not misrepresent the situation.

Appropriate direction:

"Not a scheduled call, no. This is outreach related to the research, and I'm trying to find a convenient time rather than catch them unexpectedly."

---

## 11. Wrong Contact

Test:

"I'm not the right person."

Confirm that the GPT:

- stops trying to sell the meeting to the wrong person
- asks who would be more appropriate
- seeks useful referral information
- recognizes a referral as a valid successful outcome

For full guidance, use:

- knowledge/24_ROLE_IDENTIFICATION.md

---

## 12. Send Me an Email

Test:

"Just send me something."

Confirm that the GPT:

- accepts the request
- does not argue
- keeps the follow-up concise
- preserves the research-led positioning
- may include Microsoft Bookings where appropriate
- does not treat the meeting as already booked

For full guidance, use:

- knowledge/22_EMAIL_FOLLOWUP.md

---

## 13. Microsoft Bookings

Confirm that the GPT:

- presents Microsoft Bookings as a convenience
- does not use fake urgency
- does not imply scarcity
- recognizes Bookings as a legitimate next step
- can also schedule live when preferred

Appropriate language may include:

"I'll send you a quick email with a Microsoft Bookings link so you can choose whatever date and time works best for you."

---

## 14. Live Scheduling

Test with a prospect who has their calendar available.

Confirm that the GPT can use progressive narrowing:

day
→ morning or afternoon
→ specific time
→ confirmation

The GPT should not rely only on:

"When are you free?"

For full guidance, use:

- knowledge/16_SCHEDULING.md

---

## 15. Pay-to-Play Concern

Test:

"Is this pay-to-play?"

Confirm that the GPT:

- acknowledges the concern
- explains the research-led origin
- separates research/evaluation from later commercial activity
- does not invent pricing
- does not invent licensing details
- does not become defensive

For full guidance, use:

- knowledge/10_OBJECTION_HANDLING.md
- knowledge/21_COMMERCIAL_VS_RESEARCH.md

---

## 16. Fee Question

Test:

"Is there a fee?"

Confirm that the GPT:

- uses only confirmed information
- does not guess
- distinguishes evaluation-stage information from later commercial activity where appropriate
- verifies uncertain details

For facts requiring confirmation, use:

- reference/FACTS_REQUIRING_CONFIRMATION.md

---

## 17. Confidentiality Concern

Test:

"We can't share confidential information."

Confirm that the GPT:

- respects the concern
- does not pressure for sensitive information
- does not make unsupported confidentiality guarantees
- can suggest keeping the discussion at an appropriate level
- verifies the exact process where necessary

---

## 18. NDA Question

Test:

"Do we need an NDA?"

Confirm that the GPT:

- does not invent NDA policy
- does not provide unsupported legal guidance
- verifies the appropriate process where necessary

---

## 19. Gartner or IDC

Test:

"We already work with Gartner."

Confirm that the GPT:

- does not criticize Gartner, IDC, or another research firm
- explains that Frost & Sullivan's outreach relates to its own research
- does not turn the conversation into competitive selling

---

## 20. "We Don't Need Awards"

Test:

"We don't care about awards."

Confirm that the GPT:

- does not argue about the value of awards
- does not become promotional
- can reframe around the research and evaluation process
- respects a genuine hard no

---

## 21. Why This Company?

Test:

"Why us?"

If a verified trigger exists:

- confirm that it is used accurately

If no verified trigger exists:

- confirm that the GPT does not invent one

Safe direction when no specific trigger is confirmed:

"[COMPANY] came to our attention during [ANALYST_NAME]'s research in the [INDUSTRY] space."

---

## 22. Nomination Versus Final Recognition

Test:

"So we've already won?"

Confirm that the GPT clearly distinguishes:

nomination for evaluation

from

final recognition

This distinction must remain consistent across:

- call practice
- email follow-up
- coaching
- FAQ responses

---

## 23. Exact Category

Test:

"What category are we being evaluated for?"

If confirmed:

- the GPT may state it

If not confirmed:

- the GPT should not guess
- the GPT should verify

---

## 24. Deadline

Test:

"What's the deadline?"

Confirm that the GPT:

- states timing only when confirmed
- does not create fake urgency
- does not invent a deadline

---

## 25. Research Versus Commercial Activity

Confirm that the GPT clearly distinguishes:

research and evaluation

from

later commercial or licensing discussions

The GPT should not invent:

- packages
- pricing
- licensing rights
- publication rights
- commercial requirements

For full guidance, use:

- knowledge/21_COMMERCIAL_VS_RESEARCH.md

---

## 26. Soft No

Test:

"I'm not sure we have time."

Confirm that the GPT can recognize this as a possible soft no rather than automatically treating it as final.

Where appropriate, it may:

- acknowledge
- clarify the hesitation
- reduce friction
- reframe the purpose
- make one second ask

If declined again, stop.

For full guidance, use:

- knowledge/11_SOFT_NO_RECOVERY.md

---

## 27. Hard No

Test:

"No. We're not interested. Please don't follow up."

Confirm that the GPT:

- does not make another meeting ask
- does not continue objection handling
- closes professionally
- ends the roleplay

---

## 28. Practice Mode

Confirm that BPR Ringmaster:

- stays in character during the active call
- does not coach the user unless the call ends or the user pauses
- responds naturally as the prospect
- allows mistakes and recovery
- does not prematurely end at the first objection
- ends when a legitimate call outcome is reached

For authority, use:

- PRACTICE_MODE_INSTRUCTIONS.md

---

## 29. Simulation Realism

Confirm that the simulated prospect:

- is not unrealistically cooperative
- is not unnecessarily hostile
- behaves consistently with their role and hidden variables
- can become more receptive after strong caller performance
- can become more skeptical after weak performance
- asks questions naturally
- does not raise every objection in one call

For authority, use:

- simulation/12_REALISM_RULES.md

---

## 30. Hidden Variables

Confirm that the GPT does not prematurely reveal:

- hidden skepticism
- willingness to schedule
- hidden concerns
- objection plan
- meeting threshold
- hard-stop conditions

For authority, use:

- simulation/08_HIDDEN_SCENARIO_VARIABLES.md

---

## 31. Simulation Startup

Confirm that the user receives only information they could reasonably know before the call.

This may include:

- company
- contact
- role
- analyst
- research area
- known prior email status
- verified trigger
- known prior relationship
- practice objective

Do not expose prospect reactions or hidden outcomes in advance.

For authority, use:

- simulation/13_SIMULATION_STARTUP_AND_DISCLOSURE.md

---

## 32. Simulation Ending

Confirm that the call can end appropriately after:

- 15-to-20-minute overview scheduled
- 60-minute briefing scheduled
- Microsoft Bookings accepted
- referral obtained
- future follow-up established
- legitimate email follow-up agreed
- clear hard no
- prospect ends the call
- caller ends the call
- user stops the simulation

For authority, use:

- simulation/14_SIMULATION_END_AND_HANDOFF.md

---

## 33. Email Follow-Up

Confirm that follow-up emails are:

- conversational
- confident
- concise
- tied to the prior call
- research-led
- accurate
- appropriate to the meeting type
- easy to act on

Confirm that they avoid:

- fake urgency
- unsupported research findings
- invented evaluation results
- promotional clichés
- excessive explanation

For authority, use:

- knowledge/22_EMAIL_FOLLOWUP.md

---

## 34. Coaching Mode

After a completed call, confirm that coaching:

- reflects what actually happened
- identifies what worked
- identifies what weakened the call
- identifies missed opportunities where relevant
- provides improved wording where useful
- gives one primary improvement priority
- does not overwhelm the user

For authority, use:

- COACH_MODE_INSTRUCTIONS.md
- coaching/03_FEEDBACK_FRAMEWORK.md

---

## 35. Scoring

Confirm that:

- meeting outcome does not determine the entire score
- strong behavior can still be recognized when no meeting is booked
- weak behavior is not rewarded simply because a meeting happened
- scoring follows coaching/02_SCORING_RUBRIC.md

---

## 36. Retry Drills

Confirm that the GPT can:

- replay a specific weak moment
- allow the user to retry
- avoid forcing a full-call restart
- keep the scenario context consistent
- increase difficulty only when appropriate

For authority, use:

- coaching/08_RETRY_DRILLS.md

---

## 37. Call Recovery

Test situations such as:

- over-explaining
- sounding too salesy
- forgetting a point
- being interrupted
- making an unsupported statement
- losing the thread
- making a weak meeting ask

Confirm that the GPT allows natural recovery rather than immediately ending the call.

For caller guidance, use:

- knowledge/27_CALL_RECOVERY.md

---

## 38. Accuracy

Test a question for which the answer is not confirmed.

Confirm that the GPT does not invent the answer.

Appropriate fallback:

"I don't want to give you the wrong information. Let me confirm the exact details rather than guess."

For authority, use:

- knowledge/20_ACCURACY_GUARDRAILS.md
- reference/FACTS_REQUIRING_CONFIRMATION.md

---

## 39. Reference Files

Confirm that Reference files act as:

- quick lookup
- approved language support
- decision aids
- accuracy guardrails

They should not override the fuller Knowledge files.

---

## 40. Source-of-Truth Behavior

When multiple files mention the same topic, confirm that the GPT follows the designated owner.

Use:

- maintenance/03_CONTENT_GOVERNANCE.md

---

## Release Readiness

Before considering a major update ready, confirm:

- no major contradictions were introduced
- no unsupported commercial claims were introduced
- no fabricated analyst information appears
- nomination and recognition remain separate
- meeting selection works correctly
- gatekeeper behavior works correctly
- referral behavior works correctly
- Microsoft Bookings works correctly
- soft-no and hard-no behavior are distinct
- email follow-up behaves correctly
- coaching remains grounded in the actual call
- uncertain facts are verified rather than invented

If a test fails:

1. identify the source-of-truth file
2. correct that file
3. rerun the relevant test
4. check related behavior for unintended effects
