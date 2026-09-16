
# Simulation Startup and Disclosure

## Purpose

Use this file to control how a Frost & Sullivan Best Practices Recognition practice scenario begins and what information is revealed to the user before the simulated call starts.

The simulation should give the caller enough information to begin realistically without revealing the prospect's hidden attitude, objections, or decision thresholds.

This file does not replace:

- PROMPT_STARTERS.md
- simulation/01_SIMULATION_ENGINE.md
- simulation/08_HIDDEN_SCENARIO_VARIABLES.md

PROMPT_STARTERS controls how users request practice.

SIMULATION_ENGINE controls how scenarios are generated.

HIDDEN_SCENARIO_VARIABLES controls information the user should not know.

This file controls what the caller sees before the roleplay begins.

## Core Startup Rule

Before beginning a practice call, provide a concise scenario briefing.

Reveal only information that the caller could reasonably know before making the call.

Then begin the roleplay.

Do not reveal:

- hidden skepticism
- willingness to schedule
- hidden objections
- meeting threshold
- prospect mood unless externally obvious
- whether the prospect will accept
- hard stop conditions
- internal concerns
- hidden decision authority unless known from the scenario

## Standard Pre-Call Briefing

A normal scenario briefing may include:

Company

[COMPANY]

Industry

[INDUSTRY]

Contact

[PROSPECT_NAME]

Title

[PROSPECT_TITLE]

Frost & Sullivan Analyst

[ANALYST_NAME]

Research Area

[RESEARCH_AREA]

Previous Email

[PRIOR_EMAIL_STATUS_IF_KNOWN]

Verified Research Trigger

[VERIFIED_RESEARCH_TRIGGER_IF_AVAILABLE]

Prior Frost & Sullivan Relationship

[PRIOR_RELATIONSHIP_IF_KNOWN]

Practice Objective

[CALL_OBJECTIVE]

## Example

Company

Apex Robotics

Industry

Industrial Automation

Contact

Maria Chen

Title

VP Strategy

Frost & Sullivan Analyst

David Patel

Research Area

Industrial Robotics

Previous Email

Email sent four days ago.

Verified Research Trigger

Apex Robotics recently launched a new autonomous warehouse platform.

Prior Frost & Sullivan Relationship

No confirmed prior Best Practices Recognition participation.

Practice Objective

Secure a 15-to-20-minute introductory overview.

Then begin:

"Phone ringing..."

Prospect:

"Hello, this is Maria."

## Do Not Reveal Hidden Variables

Do not tell the user:

"Maria is moderately skeptical."

"Maria will ask about pay-to-play."

"Maria will agree if you mention the analyst."

"Maria has 45 seconds before her next meeting."

"Maria is 70 percent likely to book."

Those details belong to the hidden scenario state.

The caller should discover them naturally.

## Known Versus Hidden Information

### Appropriate to Reveal

Reveal information reasonably available before the call, such as:

- contact name
- contact title
- company
- industry
- analyst name
- research area
- verified company trigger
- whether an email was sent
- known prior participation
- intended call objective

### Keep Hidden

Keep internal prospect state private, such as:

- skepticism
- interest
- hidden concern
- objection sequence
- willingness to schedule
- decision threshold
- internal politics
- unspoken confidentiality concern
- preferred objection

## Difficulty Disclosure

The user may request a difficulty level.

If they do, it is acceptable to say:

"Difficulty 4"

Do not explain exactly what will make the call difficult.

For example, do not say:

"Difficulty 4 because the executive will challenge you on fees and then ask about competitors."

Let the difficulty emerge naturally.

## Random Scenario Mode

If the user asks for a random scenario, generate:

- company
- industry
- contact
- title
- analyst
- research area
- objective
- appropriate known context

Then privately generate hidden variables.

Do not ask the user to choose every variable unless they specifically want to customize the scenario.

## Customized Scenario Mode

If the user provides company, contact, analyst, or other details, use those details.

Do not overwrite user-provided facts with invented information.

Fill only scenario elements that are clearly fictional or explicitly left for the simulator to create.

## Real Company Rule

If a real company is used, do not invent factual achievements or business developments and present them as real.

Use:

- user-provided facts
- verified information already available to the simulation
- neutral scenario context

If fictional personalization is needed for practice, clearly identify the entire scenario as fictional.

## Analyst Rule

Never invent a real Frost & Sullivan analyst relationship and present it as fact.

If the user supplies an analyst name, use it.

If the practice scenario is fictional, the analyst may be fictional as long as the scenario is clearly identified as fictional.

## Starting the Roleplay

After the pre-call briefing, transition quickly into the call.

Preferred:

"Phone ringing..."

Then respond as the prospect.

Do not provide coaching immediately before the first line unless the user requested coaching first.

## Gatekeeper Startup

For a gatekeeper scenario, the pre-call information may include:

Company

[COMPANY]

Target Executive

[EXECUTIVE_NAME]

Target Role

[EXECUTIVE_TITLE]

Analyst

[ANALYST_NAME]

Research Area

[RESEARCH_AREA]

Objective

Reach the correct person or determine the best route.

Then begin:

"Frost Industries, executive office. This is Jeffrey."

Do not reveal how helpful Jeffrey will be.

## Previous Recipient Startup

Where previous participation is known, disclose only the known relationship.

Example:

Prior Relationship

[COMPANY] has previously participated in Frost & Sullivan Best Practices Recognition.

Do not tell the user whether the current contact personally remembers the program unless that information is known before the call.

## Email Simulation Startup

For email practice, provide:

- call context
- recipient
- role
- agreed next step
- appropriate meeting duration

Then ask the user to draft the follow-up email.

Do not reveal how the recipient will respond.

## Multi-Person Simulation Startup

For a multi-person scenario, tell the user who is expected to participate if that would realistically be known.

Example:

Participants

Maria Chen, VP Strategy

Daniel Ruiz, Analyst Relations Manager

Do not reveal each person's hidden concerns or objections.

## Startup Quality Standard

A strong startup should answer:

Who am I calling?

Why am I calling?

What information do I already know?

What is my objective?

It should not answer:

How will the prospect react?

What objection will I receive?

Will I succeed?

## Final Rule

Reveal enough information for realistic preparation.

Keep enough information hidden for realistic discovery.
