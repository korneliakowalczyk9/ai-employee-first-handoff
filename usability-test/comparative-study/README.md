# Comparative study: authority labels (Version A and Version B)

An exploratory comparison of two versions of the same prototype, run remotely and without a live facilitator. It asks whether short labels at the point of action change how well people understand what an AI employee may do, what needs their approval and how much control they keep.

This is a small within-subject comparison with six participants. It is not a statistically conclusive A/B test.

## How this study uses the test plan

The general [test plan](../test-plan.md) is the authority for the remote procedure, the evidence rules, the planted-error rules, the support messages, recording review and the limitations of unmoderated testing. This page defines only what is specific to the comparison. Where the general study (five participants, one version) and this study differ, this page governs the comparative study. See [../README.md](../README.md) for how the two studies differ.

## Hypothesis

Adding a short authority label at the moment of each action, on top of the upfront explanation, helps participants say more accurately what Aria may do on its own and what needs their approval, compared with the upfront explanation alone.

This is a question, not a prediction. "No difference" and "worse" are acceptable results. The study also looks at whether the labels change how in control and how comfortable participants feel.

## The treatment

**Point-of-action authority labels: present (Version B) or absent (Version A).**

| | Version A | Version B |
|---|---|---|
| What it is | The existing baseline wireframes and Figma prototype, unchanged | The same screens with labels added |
| Upfront explanation | Yes. Limits are on the first screen and the access pop-up and send dialog explain approval | Yes, identical |
| Labels at the point of action | None | Yes, listed below |

Version A is the existing screens in `design/version-a/` and the existing Figma prototype. Version B is in `design/version-b/` and in a separate Figma prototype. Both are Figma research prototypes.

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

Unchanged in Version B: the Maya scenario, the 12 fictional requests, the four drafts, the planted Thursday/Friday error, the access, stop, edit and send rules, the timers and all other wording and interactions.

There are two documented differences between the versions:
1. The authority labels.
2. A layout consequence of the labels. On the results screens the Lena and Sam cards each gain one muted line, about 23 px of height, which moves the content below them down. The results screens are 1253 px tall in Version B and 1230 px in Version A.

The study cannot separate the labels from the 23 px taller cards. It tests the label-and-presentation treatment as implemented, not the labels alone.

## Design

- Six participants. Each sees both versions, one after the other.
- Order alternates. Three participants see A then B and three see B then A.
- Participants are told "Version 1" and "Version 2", never A or B. Version 1 is whatever they open first. Only the researcher knows which is which.
- After each version the participant answers the same questions. The comparison questions come once, at the end.
- The participant must finish Version 1 and its questions before opening Version 2. The form's pages enforce the sequence.

| Participant | Sees first (Version 1) | Sees second (Version 2) |
|---|---|---|
| P1 | A | B |
| P2 | B | A |
| P3 | A | B |
| P4 | B | A |
| P5 | A | B |
| P6 | B | A |

If a participant drops out or does not finish both versions, replace them with a new person in the same slot so the order stays balanced. The criteria for participants are in the test plan.

### A participant's journey, about 40 minutes

| Step | Time | What happens |
|---|---|---|
| 1. Information and consent | 3 min | The participant reads the information and chooses whether to record. Recording is optional. |
| 2. Background | 2 min | Familiarity with conversational AI, asked once. |
| 3. Version 1 | 12 min | The participant uses the first prototype alone. |
| 4. Questions about Version 1 | 6 min | D3 first, then Blocks A to D of the questionnaire. |
| 5. Version 2 | 8 min | The same scenario again, in the other version. |
| 6. Questions about Version 2 | 6 min | The same questions. |
| 7. Final comparison | 3 min | Part 4, answered after both. |

## Primary evidence is the first exposure

The second version is affected by learning and by the questions asked after the first version. The participant has already seen the screens, the task and the prototype, and has answered the knowledge check and the reflection questions. So:

- **Primary comparison:** first-exposure evidence and responses. Participants 1, 3 and 5 saw A first and 2, 4 and 6 saw B first. Compare these two groups.
- **Supplementary evidence:** second-exposure results. They are useful, but they are not independent measurements of the label effect. Read each participant's A against B as affected by order, learning and questionnaire priming. It can support a first-exposure difference but cannot establish one on its own.
- **Planted error:** counted only on the first exposure. On the second exposure the participant already knows the content, so do not count noticing, acting on it or the reasons for sending.

Neither the questionnaire nor the researcher reveals correct answers or explains product rules between versions. Answers are scored after all responses are in. With six people, do not present average ratings or a simple Version 1 against Version 2 score as conclusive. Individual responses, explanations and any recorded behaviour matter most.

## What the results can and cannot tell us

**Can:**
- Whether a pattern appears in the same direction for most participants.
- How participants describe the boundaries of what Aria may do.
- Which statements people get wrong in each version.
- Where confusion, hesitation and misreadings happen, as far as the recordings and answers show.

**Cannot:**
- Show statistical significance or the size of any effect.
- Generalise beyond six people, this prototype and this scenario.
- Separate the effect of the labels from the effect of seeing the task twice or of answering the questionnaire after the first version.
- Show that the labels caused a difference rather than the extra information they add. Version B has more text than Version A.
- Isolate the labels from the 23 px taller results cards.
- Show what participants did without a recording, or what any participant noticed or thought, even with one.

Treat any finding as a question for a next round.

## Weaknesses specific to this design

The general limitations of unmoderated testing, self-report, optional recordings and the prototype (no real AI execution, no interaction analytics, no completed correction) are in the [test plan](../test-plan.md#limitations-of-unmoderated-remote-testing) and apply here.

- **Carryover:** The second run benefits from the first, even with alternating order.
- **Questionnaire priming:** The knowledge check and the reflection questions after the first version may change how participants approach the second one. Having answered what Aria does on its own and what needs approval, a participant may start looking for that information in the second version. Alternating the order does not remove this. It is why first-exposure results are primary and paired results carry less weight.
- **More information:** Version B adds information, so a difference may come from the amount and not only the position.
- **Layout difference:** Version B's results cards are 23 px taller. The study cannot tell the labels apart from this change.
- **Salience of Send:** The "Approval required to send" label might make Send more noticeable. Check this in the evidence that exists, and treat it with caution.
- **Small numbers:** Three participants per order group.

## Prototypes

Interactive Figma prototypes of the two versions. They are for the researcher. Participants are given links labelled "Version 1" and "Version 2" and are never told which is which.

| Version | Prototype | Screens |
|---|---|---|
| A | [Open Prototype A](https://www.figma.com/proto/kqTE0fRgfgt9hXtxeuyTJx?page-id=35%3A2&node-id=36-23&starting-point-node-id=36-23) | [design/version-a/](../../design/version-a/README.md) |
| B | [Open Prototype B](https://www.figma.com/proto/kqTE0fRgfgt9hXtxeuyTJx?page-id=44%3A5722&node-id=44-5723&starting-point-node-id=44-5723) | [design/version-b/](../../design/version-b/README.md) |

Both start at the first screen, "Task and limits".

## Materials

- [../test-plan.md](../test-plan.md): procedure, evidence rules, running the studies and decisions before recruiting
- [../evidence-record.md](../evidence-record.md): one record per exposure
- [comparison-and-findings-template.md](comparison-and-findings-template.md): scoring and comparing the results, with the answer key (researcher only)
- [../online-questionnaire.md](../online-questionnaire.md): questionnaire wording
- [../participant-materials/](../participant-materials/): instructions and the information and consent page
