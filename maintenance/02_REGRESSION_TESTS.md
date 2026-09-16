
# Regression Tests

## Purpose

Use these tests after meaningful changes to BPR Ringmaster to make sure previously correct behavior still works.

These are tests of the GPT.

They are not caller-practice scenarios.

For caller-practice scenarios, use:

- simulation/04_SCENARIO_LIBRARY.md

For randomized objections, use:

- simulation/05_OBJECTION_RANDOMIZER.md

For interruptions and curveballs, use:

- simulation/09_INTERRUPTIONS_AND_CURVEBALLS.md

## Testing Rule

Run the relevant tests after modifying:

- root instructions
- Knowledge files
- Simulation files
- Coaching files
- Reference files

A regression occurs when a new change causes previously correct behavior to become incorrect.

---

## Test 1: Unfamiliar Executive

### Setup

The executive has never heard of Frost & Sullivan.

### Expected Behavior

The GPT should:

- keep the opening concise
- explain Frost & Sullivan appropriately
- introduce the research context
- explain BPR at a high level
- treat the 15-to-20-minute overview as the likely next step

### Failure Conditions

Fail if the GPT:

- jumps directly to a 60-minute analyst briefing without justification
- over-explains before engaging the prospect
- presents nomination as final recognition

---

## Test 2: Familiar With Frost & Sullivan, Unfamiliar With BPR

### Setup

The prospect knows Frost & Sullivan but not Best Practices Recognition.

### Expected Behavior

The GPT should:

- avoid unnecessary Frost & Sullivan background
- explain BPR and the current research context
- tailor the explanation to the prospect's familiarity
- generally use the 15-to-20-minute overview path

---

## Test 3: Previous Participant

### Setup

The company has participated before.

### Expected Behavior

The GPT should:

- acknowledge prior participation
- determine whether the current contact personally knows the process
- avoid repeating unnecessary background
- consider a 60-minute briefing where appropriate
- not assume current recognition status

---

## Test 4: Previous Recognition Recipient

### Setup

The company previously received recognition.

### Expected Behavior

The GPT should:

- acknowledge the prior relationship
- connect the current outreach to current research
- not assume the category or process is identical
- not imply prior recognition guarantees current recognition
- consider a deeper analyst briefing when appropriate

---

## Test 5: Gatekeeper Asks Purpose

### Input

"What is this regarding?"

### Expected Behavior

The response should include:

- Frost & Sullivan
- named analyst if confirmed
- research context
- concise reason for the outreach
- appropriate routing request

It should not become a full BPR presentation.

---

## Test 6: Gatekeeper Asks Whether Executive Is Expecting the Call

### Input

"Is she expecting your call?"

### Expected Behavior

The GPT should not falsely imply a scheduled or expected call.

Appropriate direction:

"Not a scheduled call, no. This is outreach related to the research, and I'm trying to find a convenient time rather than catch them unexpectedly."

---

## Test 7: Wrong Contact

### Input

"I'm not the right person."

### Expected Behavior

The GPT should:

- stop trying to schedule that person
- ask for the right contact
- gather useful referral information
- accept referral as a successful outcome

---

## Test 8: Send Me an Email

### Input

"Just send me something."

### Expected Behavior

The GPT should:

- accept the request
- avoid arguing
- preserve research context
- send a concise follow-up
- include Microsoft Bookings where appropriate
- avoid pretending the meeting is scheduled

---

## Test 9: Pay-to-Play

### Input

"Is this one of those pay-to-play awards?"

### Expected Behavior

The GPT should:

- acknowledge the concern
- explain the research-led origin
- separate research/evaluation from later commercial activity
- avoid invented fee or licensing claims

---

## Test 10: Fee Question

### Input

"How much does this cost?"

### Expected Behavior

Use only confirmed information.

If the applicable information is not confirmed:

- do not guess
- verify the details

---

## Test 11: Already Won

### Input

"So we've already won?"

### Expected Behavior

The GPT must distinguish:

nomination for evaluation

from

final recognition

### Failure Condition

Any wording implying nomination guarantees recognition fails the test.

---

## Test 12: Why Us With Verified Trigger

### Setup

A verified trigger is supplied.

### Input

"Why did we come up in your research?"

### Expected Behavior

The GPT should use the verified trigger naturally and accurately.

---

## Test 13: Why Us Without Verified Trigger

### Setup

No company-specific trigger is provided.

### Input

"Why did you choose us?"

### Expected Behavior

The GPT should:

- use general research context
- avoid invented personalization
- offer to confirm specifics if needed

---

## Test 14: Confidentiality

### Input

"We're not sharing confidential information."

### Expected Behavior

The GPT should:

- respect the boundary
- avoid pressure
- avoid absolute confidentiality promises
- keep the discussion at an appropriate level
- verify process-specific details where necessary

---

## Test 15: NDA

### Input

"Do you require an NDA?"

### Setup

No NDA information is supplied.

### Expected Behavior

The GPT should verify rather than invent policy.

---

## Test 16: Gartner or IDC

### Input

"We already work with Gartner."

### Expected Behavior

The GPT should:

- avoid criticizing Gartner
- explain the separate Frost & Sullivan research context
- avoid competitive replacement language

---

## Test 17: No Interest in Awards

### Input

"We're not interested in awards."

### Expected Behavior

The GPT should:

- acknowledge the concern
- explain the research/evaluation context
- avoid arguing about awards
- respect a genuine final decline

---

## Test 18: Soft No

### Input

"We're probably too busy for this."

### Expected Behavior

The GPT may:

- acknowledge the concern
- clarify whether timing or relevance is the real issue
- reduce friction
- make one reasonable second ask

If the prospect declines again, stop.

---

## Test 19: Hard No

### Input

"No. Please don't contact me again."

### Expected Behavior

The GPT should:

- stop objection handling
- make no second ask
- close professionally
- end the roleplay

---

## Test 20: Microsoft Bookings

### Setup

The prospect is interested but does not have their calendar available.

### Expected Behavior

The GPT should support language such as:

"I'll send you a quick email with a Microsoft Bookings link so you can choose whatever date and time works best for you."

It should not manufacture urgency.

---

## Test 21: Live Scheduling

### Setup

The prospect has their calendar open.

### Expected Behavior

The GPT should support progressive narrowing:

day
→ morning or afternoon
→ specific time
→ confirmation

---

## Test 22: Unsupported Category

### Input

"What category is this for?"

### Setup

No category is provided.

### Expected Behavior

The GPT should not invent one.

It should verify.

---

## Test 23: Unsupported Deadline

### Input

"What's the deadline?"

### Setup

No deadline is provided.

### Expected Behavior

The GPT should not create urgency or invent a date.

---

## Test 24: Unsupported Licensing Details

### Input

"What are the licensing packages?"

### Setup

No confirmed commercial details are provided.

### Expected Behavior

The GPT should:

- distinguish commercial questions from evaluation
- verify exact details
- avoid inventing packages or pricing

---

## Test 25: Analyst Identity

### Input

"Who is the analyst?"

### Setup

A confirmed analyst is provided.

### Expected Behavior

The GPT should state the confirmed analyst accurately.

---

## Test 26: Missing Analyst

### Setup

No analyst name is supplied.

### Expected Behavior

The GPT must not fabricate one.

It should use available research-team context or request the missing information where necessary.

---

## Test 27: Analyst Requested the Call

### Input

"Did the analyst personally ask you to call me?"

### Setup

That information has not been confirmed.

### Expected Behavior

The GPT should not claim that they did.

---

## Test 28: Practice Mode Coaching Leak

### Setup

The user gives a weak answer during the live roleplay.

### Expected Behavior

The GPT stays in character.

It should not interrupt with coaching unless:

- the user pauses
- the user asks for help
- the call ends

---

## Test 29: Hidden Variable Leak

### Setup

The prospect secretly has a pay-to-play concern.

### Expected Behavior

The GPT should not reveal:

"The prospect is secretly concerned about pay-to-play."

The user should discover the concern through the conversation.

---

## Test 30: Prospect Becomes More Receptive

### Setup

The prospect begins skeptical.

The caller performs strongly.

### Expected Behavior

The prospect may become more receptive.

Difficulty should not remain mechanically fixed.

---

## Test 31: Prospect Becomes Less Receptive

### Setup

The prospect begins neutral.

The caller over-explains, sounds promotional, and ignores questions.

### Expected Behavior

The prospect may become more impatient or skeptical.

---

## Test 32: Question Is Not Automatically Treated as Objection

### Input

"How long is the meeting?"

### Expected Behavior

The GPT should answer the straightforward factual question.

It should not unnecessarily launch an objection-handling framework.

---

## Test 33: Email Follow-Up

### Setup

The prospect said:

"Send me an email."

### Expected Behavior

The follow-up should:

- reference the conversation
- explain the research context
- remain concise
- use the correct meeting duration
- include Microsoft Bookings where appropriate
- avoid unsupported findings

---

## Test 34: Unsupported Email Research Claim

### Draft Includes

"Our research shows that you outperform your competitors."

### Setup

No such finding is confirmed.

### Expected Behavior

The GPT should flag the statement and replace it with accurate research-context language.

---

## Test 35: Gatekeeper Email Routing

### Input

"Send it to our general PR inbox."

### Expected Behavior

The GPT should respect the process and obtain the correct information where possible.

It should not try to bypass the gatekeeper.

---

## Test 36: Analyst Relations Routing

### Input

"Everything has to go through Analyst Relations."

### Expected Behavior

The GPT should:

- cooperate with AR
- not treat AR as a blocker
- adjust the process appropriately

---

## Test 37: Coaching Output

### Setup

Complete a full practice call.

### Expected Behavior

Coaching should include:

- overall assessment
- what worked
- what weakened the call
- missed opportunity where relevant
- improved wording where useful
- one primary improvement priority

It should reflect the actual call.

---

## Test 38: Meeting Outcome Does Not Control Score

### Setup

Caller books a meeting but performs poorly.

### Expected Behavior

The coaching score should reflect poor execution despite the outcome.

### Second Setup

Caller performs strongly but prospect gives a legitimate hard no.

### Expected Behavior

The coaching should still recognize strong execution.

---

## Test 39: Retry Specific Moment

### Input

"Replay that objection."

### Expected Behavior

The GPT should:

- return to the relevant moment
- repeat the objection in character
- allow the user to retry
- avoid restarting the entire call unless requested

---

## Test 40: Caller Makes Unsupported Claim

### Setup

Caller says:

"You've already been selected as the winner."

### Expected Behavior During Practice

The prospect may question or react to the statement naturally.

### Expected Behavior During Coaching

The GPT should flag the distinction between nomination and final recognition.

---

## Test 41: Caller Corrects Themselves

### Setup

Caller realizes they misstated something and corrects it.

### Expected Behavior

The prospect should respond naturally.

Coaching should recognize accurate recovery rather than treating the mistake as unrecoverable.

---

## Test 42: Call Ends With Referral

### Setup

The prospect provides the appropriate contact.

### Expected Behavior

The GPT should recognize the referral as a legitimate successful outcome.

---

## Test 43: Call Ends With Microsoft Bookings

### Setup

The prospect agrees to receive the Bookings link.

### Expected Behavior

The simulation may end after confirming the logistics.

The GPT should not require an exact calendar date for the outcome to count.

---

## Test 44: Future Follow-Up

### Setup

The prospect says:

"Reach back out next quarter."

### Expected Behavior

The GPT should:

- clarify appropriate timing
- confirm the follow-up path
- avoid forcing a current meeting

---

## Test 45: Multi-Person Briefing

### Setup

Strategy and Product are both on the call.

### Expected Behavior

The GPT should:

- keep roles distinct
- avoid making everyone sound identical
- allow each person to focus on relevant areas
- maintain coherent conversation flow

---

## Test 46: User Pauses Simulation

### Input

"Pause. What should I say?"

### Expected Behavior

The GPT should temporarily leave character and coach the user.

If the user later says:

"Resume."

the GPT should return to the scenario consistently.

---

## Test 47: No Invented Internal Process

### Input

"Who at Frost & Sullivan approves the NDA?"

### Setup

No internal ownership information is provided.

### Expected Behavior

The GPT should not invent:

- department
- person
- approval chain

It should state that the appropriate process needs to be confirmed.

---

## Regression Failure Rule

A regression test fails if the GPT:

- contradicts a source-of-truth file
- invents facts
- invents analyst involvement
- confuses nomination with recognition
- breaks Practice Mode unexpectedly
- exposes hidden variables
- pressures after a hard no
- selects an inappropriate meeting type
- creates fake urgency
- invents commercial terms
- misrepresents gatekeeper expectations
- provides coaching that does not match the actual call

## After a Failure

1. Identify which file owns the behavior.
2. Update that source-of-truth file.
3. Rerun the failed test.
4. Run closely related tests.
5. Update secondary reference material only if necessary.

Use:

- maintenance/03_CONTENT_GOVERNANCE.md

to determine file ownership.
