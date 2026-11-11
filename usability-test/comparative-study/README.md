# Comparative study: authority labels (Version A and Version B)

An exploratory comparison of two versions of the same prototype. It asks whether short labels at the point of action change how well people understand what an AI employee may do, what needs their approval and how much control they keep.

This is a small within-subject comparison with six participants. It is not a statistically conclusive A/B test.

## How this study uses the general test plan

The general usability test (five participants, one version) is a separate study. See [../README.md](../README.md) for how the two studies differ.

- The general [test plan](../test-plan.md) applies to both studies for the standard session procedure: who takes part, the setup, the introduction, the scenario, the participant-led walkthrough, the neutral prompts and what the facilitator must not do. That procedure is not repeated here.
- The materials in this folder govern version order, participant responses, observations and analysis for the comparative study: the [facilitator guide](facilitator-guide.md), the [participant response template](participant-response-template.md), the [observation sheet](observation-sheet.md) and the [findings template](comparison-and-findings-template.md).
- The general study's five-participant, one-version design does not govern this study. Where the two differ, this folder governs the comparative study.

Differences from the standard session procedure:
- Six participants, with the same criteria as the general test plan.
- The introduction has one extra sentence, given in the facilitator guide.
- Each participant uses two versions, one after the other.
- The general plan's post-task questions are replaced by the participant response template (Sections 1 and 2, after each version) and a short spoken comparison (Section 3, after both).
- The session takes about 50 minutes instead of 30.

## Hypothesis

Adding a short authority label at the moment of each action, on top of the upfront explanation, helps participants say more accurately what Aria may do on its own and what needs their approval, compared with the upfront explanation alone.

This is a question, not a prediction. "No difference" and "worse" are acceptable results. The study also looks at whether the labels change how in control and how comfortable participants feel.

## The treatment

**Point-of-action authority labels: present (Version B) or absent (Version A).**

| | Version A | Version B |
|---|---|---|
| What it is | The existing baseline wireframes and prototype, unchanged | The same screens with labels added |
| Upfront explanation | Yes. Limits are on the first screen and the access pop-up and send dialog explain approval | Yes, identical |
| Labels at the point of action | None | Yes, listed below |

Version A is not copied. It is the existing screens in `design/version-a/` and the existing prototype. Version B is in `design/version-b/` and in a separate prototype.

### Labels in Version B

The labels are muted text in the same style as existing hint text, in fixed positions. They are not buttons and they do not draw attention to Send.

| Where | Label |
|---|---|
| Plan, step 1 (read the inbox and the board) | Read-only access |
| Plan, step 2 (sort and flag) | No changes to requests |
| Plan, step 3 (write draft replies) | Drafts remain private |
| Sorting screens (working, stop requested) | No changes to requests |
| Drafting screens (working, after resume, stop in last stage) | Drafts remain private |
| Lena's and Sam's draft cards, next to Send | Approval required to send |

"No changes to requests" means the original requests are not modified. Sorting and ranking still happen.

"Approval required to send" shows only on a card whose Send button is available. It disappears only from the card of the reply that has been sent. The other reply keeps its label until it is sent too, so nothing suggests that approval is no longer needed for an unsent reply.

### What stays the same, and what does not

Unchanged in Version B: the Maya scenario, the 12 fictional requests, the four drafts, the planted Thursday/Friday error, the access, stop, edit and send rules, the facilitator-controlled editing step, the timers and all other wording and interactions.

There are two documented differences between the versions:
1. The authority labels.
2. A layout consequence of the labels. On the results screens the Lena and Sam cards each gain one muted line, about 23 px of height, which moves the content below them down. The results screens are 1253 px tall in Version B and 1230 px in Version A.

The study cannot separate the labels from the 23 px taller cards. It tests the label-and-presentation treatment as implemented, not the labels alone.

## Design

- Six participants. Each sees both versions, one after the other.
- Order alternates. Three participants see A then B and three see B then A.
- Participants are told "Version 1" and "Version 2", never A or B. Version 1 is whatever they see first.
- In each version the participant does the whole task, then answers the same questions.
- Only the facilitator knows which version is which.

| Participant | Sees first (Version 1) | Sees second (Version 2) |
|---|---|---|
| P1 | A | B |
| P2 | B | A |
| P3 | A | B |
| P4 | B | A |
| P5 | A | B |
| P6 | B | A |

If a participant drops out, replace them with a new person in the same slot so the order stays balanced.

### A session, about 50 minutes

| Part | Time | What happens |
|---|---|---|
| 1. Introduction | 5 min | The standard introduction plus one sentence. Ask for permission to record. |
| 2. First version, full task | 15 min | The participant does the whole task, thinking aloud. The facilitator stays silent. |
| 3. Questions after the first version | 6 min | Section 1 of the response template: knowledge check, five ratings, two open questions. |
| 4. Second version, full task | 8 min | The same scenario again, with a short instruction. |
| 5. Questions after the second version | 6 min | Section 2 of the response template, with the same questions. |
| 6. Comparison | 5 min | Section 3, answered aloud. The facilitator writes the answers down. |
| 7. Close | 2 min | Thank the participant. |

## Evidence, in three separate kinds

| Kind | What it is | How it is collected |
|---|---|---|
| Observed behaviour | What the participant does and says while working | The facilitator's observation sheet |
| Tested understanding | Whether they identify correctly what Aria does alone, what needs approval and what it cannot do | An 8-statement knowledge check, scored after the sessions |
| Stated opinion | How they say they feel | Five ratings and open comments |

Keep these apart when analysing. A participant may say they felt in control and still misunderstand an approval, or the reverse. Do not combine the four planted-error observations into one trust score.

## Primary evidence is the first exposure

The second version is affected by learning and by the questions asked after the first version. The participant has already seen the screens, the task and the prototype, and has answered the knowledge check and the reflection questions. So:

- **Primary comparison:** first-exposure observations and responses. Participants 1, 3 and 5 saw A first and 2, 4 and 6 saw B first. Compare these two groups.
- **Supplementary evidence:** second-exposure results. They are useful, but they are not independent measurements of the label effect. Read each participant's A against B as affected by order, learning and questionnaire priming. It can support a first-exposure difference but cannot establish one on its own.
- **Planted error:** counted only on the first exposure. On the second exposure the participant already knows the content, so do not count noticing, correcting or the reasons for sending.

Neither the questionnaire nor the facilitator reveals correct answers or explains product rules between versions. Answers are scored after all sessions.

With six people, do not present average ratings or a simple Version 1 against Version 2 score as conclusive. Individual responses, explanations and observed behaviour matter most.

## What the results can and cannot tell us

**Can:**
- Whether a pattern appears in the same direction for most participants.
- How participants describe the boundaries of what Aria may do.
- Which statements people get wrong in each version.
- Where confusion, hesitation and misreadings happen.

**Cannot:**
- Show statistical significance or the size of any effect.
- Generalise beyond six people, this prototype and this scenario.
- Separate the effect of the labels from the effect of seeing the task twice or of answering the questionnaire after the first version.
- Show that the labels caused a difference rather than the extra information they add. Version B has more text than Version A.
- Isolate the labels from the 23 px taller results cards.

Treat any finding as a question for a next round.

## Known weaknesses

- **Carryover:** The second run benefits from the first, even with alternating order.
- **Questionnaire priming:** The knowledge check and the reflection questions after the first version may change how participants approach the second one. Having answered what Aria does on its own and what needs approval, a participant may start looking for that information in the second version. This adds to learning and alternating the order does not remove it. It is why first-exposure results are the primary evidence and why paired results carry less weight.
- **More information:** Version B adds information, so a difference may come from the amount and not only the position.
- **Layout difference:** Version B's results cards are 23 px taller. The study cannot tell the labels apart from this change.
- **Salience of Send:** The "Approval required to send" label might make Send more noticeable. Watch for this.
- **Small numbers:** Three participants per order group.

## Prototypes

Interactive Figma prototypes of the two versions. They are for the facilitator. Participants are told "Version 1" and "Version 2" and never see which link is which.

| Version | Prototype | Screens |
|---|---|---|
| A | [Open Prototype A](https://www.figma.com/proto/kqTE0fRgfgt9hXtxeuyTJx?page-id=35%3A2&node-id=36-23&starting-point-node-id=36-23) | [design/version-a/](../../design/version-a/README.md) |
| B | [Open Prototype B](https://www.figma.com/proto/kqTE0fRgfgt9hXtxeuyTJx?page-id=44%3A5722&node-id=44-5723&starting-point-node-id=44-5723) | [design/version-b/](../../design/version-b/README.md) |

Both start at the first screen, "Task and limits". Press **R** at any time to reset. The facilitator keys are in [facilitator-guide.md](facilitator-guide.md).

## Materials

- [../test-plan.md](../test-plan.md): the standard session procedure, shared with the general usability test
- [facilitator-guide.md](facilitator-guide.md): rules and instructions for this study, including what to say and the order of exposure
- [participant-response-template.md](participant-response-template.md): what the participant answers
- [observation-sheet.md](observation-sheet.md): what the facilitator records while observing
- [comparison-and-findings-template.md](comparison-and-findings-template.md): scoring and comparing the results
- Version B screens: [design/version-b/](../../design/version-b/README.md)
