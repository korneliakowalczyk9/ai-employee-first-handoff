# Comparative study: authority labels (Version A and Version B)

An exploratory comparison of two versions of the same prototype. It asks whether short labels at the point of action change how well people understand what an AI employee may do, what needs their approval and how much control they keep.

This is a small within-subject comparison with six participants. It is not a statistically conclusive A/B test.

The general usability test (five participants) is a separate study. Its test plan, facilitator guide and note template are in the parent folder and stay as they are. This comparative study has six participants and its own materials in this folder. See [../README.md](../README.md) for how the two studies differ.

## Hypothesis

Adding a short authority label at the moment of each action, on top of the upfront explanation, helps participants say more accurately what Aria may do on its own and what needs their approval, compared with the upfront explanation alone.

This is a question, not a prediction. "No difference" and "worse" are acceptable results. The study also looks at whether the labels change how in control and how comfortable participants feel.

## The one design variable

**Point-of-action authority labels: present (Version B) or absent (Version A).**

| | Version A | Version B |
|---|---|---|
| What it is | The existing approved wireframes and prototype, unchanged | The same screens with labels added |
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

The "Approval required to send" label shows only while a card's Send button is available. Once a reply is sent, the card shows "Sent (simulated)" and no label.

### What stays identical

Everything else: the Maya scenario, the 12 fictional requests, the four drafts, the planted Thursday/Friday error, the access, stop, edit and send rules, the facilitator-controlled editing step, the timers and all other wording and interactions are unchanged. The labels are the only intended change. They have one documented layout consequence: on the results screens the Lena and Sam cards each gain one muted line, about 23 px of height, which moves the content below them down. The results screens are 1253 px tall in Version B and 1230 px in Version A.

## Design

- Six participants. Each sees both versions, one after the other.
- Order alternates. Participants 1, 3 and 5 see A then B. Participants 2, 4 and 6 see B then A.
- Participants are told "Version 1" and "Version 2", never A or B. Version 1 is whatever they see first.
- In each version the participant does the whole task, then answers the same questions.

## Evidence, in three separate kinds

| Kind | What it is | How it is collected |
|---|---|---|
| Observed behaviour | What the participant does and says while working | The facilitator's observation sheet |
| Tested understanding | Whether they identify correctly what Aria does alone, what needs approval and what it cannot do | An 8-statement knowledge check, scored after the sessions |
| Stated opinion | How they say they feel | Five ratings and open comments |

Keep these apart when analysing. A participant may say they felt in control and still misunderstand an approval, or the reverse.

## Primary evidence is the first exposure

The second version is affected by learning and by the questions asked after the first version. The participant has already seen the screens, the task and the prototype, and has answered the knowledge check and the reflection questions. So:

- **Primary comparison:** first-exposure results. Participants 1, 3 and 5 saw A first and 2, 4 and 6 saw B first. Compare these two groups.
- **Secondary comparison:** each participant's scores in A against B. Read it as affected by order, learning and questionnaire priming. It can support a first-exposure difference but cannot establish one on its own.
- **Planted error:** counted only on the first exposure. On the second exposure the participant already knows the content, so do not count noticing, correcting or the reasons for sending.

Neither the questionnaire nor the facilitator reveals correct answers or explains product rules between versions. Answers are scored after all sessions.

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

Treat any finding as a question for a next round.

## Known weaknesses

- **Carryover:** The second run benefits from the first, even with alternating order.
- **Questionnaire priming:** The knowledge check and the reflection questions after the first version may change how participants approach the second one. Having answered what Aria does on its own and what needs approval, a participant may start looking for that information in the second version. This adds to learning and alternating the order does not remove it. It is why first-exposure results are the primary evidence and why paired results carry less weight.
- **More information:** Version B adds information, so a difference may come from the amount and not only the position.
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

- [test-plan.md](test-plan.md): how a session runs
- [participant-response-template.md](participant-response-template.md): what the participant answers
- [observation-sheet.md](observation-sheet.md): what the facilitator records while observing
- [facilitator-guide.md](facilitator-guide.md): rules and instructions
- [comparison-and-findings-template.md](comparison-and-findings-template.md): scoring and comparing the results
- Version B screens: [design/version-b/](../../design/version-b/README.md)
