# Remote usability test plan

This plan is for the researcher. It is the source of the standard procedure for both studies. Participant-facing text is kept separately in [participant-materials/](participant-materials/).

A remote, unmoderated test of the interactive Figma prototype. Each participant works alone, with no live facilitator. It checks whether people can hand a first task to an AI employee and feel in control while doing it. It tests the design, not the participant.

Everything in the prototype is fictional and simulated. The prototype is not a real AI employee.

The [comparative study](comparative-study/README.md) reuses this procedure and adds its own materials. The two studies keep separate participants, evidence and findings.

## What changed from the earlier moderated plan

The earlier plan assumed a facilitator who watched, prompted and showed the result of an edit. Both studies are now remote and unmoderated (decision 38), so participants work alone and nothing is observed live. Behaviour is seen only through optional screen recordings, and understanding is collected afterwards in the questionnaire as self-report. The prototype cannot demonstrate a successful correction, so the objective is error awareness and sending decisions (decision 39). This plan is not the old procedure renamed.

## The two studies

| | General usability test | Comparative study |
|---|---|---|
| Participants | Five | Six |
| What they see | One version: Version A, the baseline | Both versions, one after the other |
| Participant instructions | [general-study-instructions.md](participant-materials/general-study-instructions.md) | [comparative-study-instructions.md](participant-materials/comparative-study-instructions.md) |
| Questionnaire | Parts 1 and 2, then Blocks A to E | Parts 1 and 2, Blocks A to D after each version, then Part 4 |
| Evidence record | [evidence-record.md](evidence-record.md) | [evidence-record.md](evidence-record.md), one per exposure |

All questionnaire wording is in [online-questionnaire.md](online-questionnaire.md).

## Participants

- Five adults for the general study and six for the comparative study. Use different people for each study.
- Adults who use chat AI tools such as ChatGPT.
- None has handed real work to an AI employee before.
- None works on this project or knows the planted error.
- Use no confidential information from any workplace.
- Participants need a computer with a current browser. The prototype is designed for a desktop screen.

## What we want to learn

1. Does the participant understand what the AI will do and what it will not do?
2. Is it clear what the AI can read?
3. Can they follow what the AI is doing without a technical log?
4. Do they notice the mistake in a draft without being told and do they act on it?
5. Is sending available without being pushed? Do they decide to send and why?
6. If they use Stop or "Not now", do they understand what happens?

Question 4 now asks whether they act on it. The prototype cannot show a corrected draft, so we record what they say they would change, whether they opened the edit screen and whether they tried to save. We cannot record a completed correction, and the prototype cannot demonstrate a successful one.

## How a participant takes part

1. Participant codes and the comparative order allocation are prepared in advance, before recruiting. When someone agrees to take part, the researcher gives them the next unused code and sends the instructions, the information page and the matching form link. The code fixes the order, so the researcher never chooses it for a particular person.
2. The participant reads the information and consents, and chooses whether to record.
3. The participant answers the background questions.
4. The participant opens the prototype link and uses it alone, as described in the instructions.
5. The participant answers the questionnaire about the experience.
6. If they recorded, they send the recording by the route decided in advance.

There is no contact between the researcher and the participant during the task, apart from technical support. See [Support messages](#support-messages).

## Evidence

Every finding is recorded with its source. Keep these sources apart.

| Source | What it can show | What it cannot show |
|---|---|---|
| **Recording (R)**, if the participant provides one | What was on the screen, what they clicked, in what order and for how long. Unexpected screen changes. | What they were thinking, noticing or intending. It is screen only, with no voice or face. |
| **Prototype data (P)** | Nothing. There is no tracking in the prototype and Figma gives no per-participant interaction data here. Do not plan for it. | Everything. Treat this source as not available. |
| **Self-report (S)** | What the participant says they did, understood or felt, in the questionnaire. This includes the knowledge check, which measures reported understanding. | What they actually did or understood. People forget, tidy up and misremember. The knowledge check is not observed behaviour. |
| **Researcher interpretation (I)** | What the researcher thinks it means. Kept in its own field. | It is not evidence. |
| **Missing (U)** | Nothing. | The finding is unknown. |

Rules for recording evidence:

- Write each finding with its value and its source, for example "Opened Sam's edit screen (R)" or "Says they noticed it while reading (S)".
- Never write a self-reported action as an observed action. "Participant says they pressed Stop" is self-report. "Participant pressed Stop" needs a recording.
- **Unknown is a legitimate value.** If there is no evidence either way, record Unknown. It is not a failure and it is not a success.
- A recording can show an action consistent with noticing, such as opening Sam's edit screen. It cannot confirm that the participant noticed something.
- Quote the participant's exact words and note where they came from: the question ID or the recording time.
- Do not infer trust, competence or understanding from a failure to notice the planted error.
- The five ratings (C1 to C5) measure different things: perceived understanding of what Aria may do, perceived understanding of approval, control, comfort and clarity of the workflow. Analyse them separately and never add them into a composite score. See [online-questionnaire.md](online-questionnaire.md).
- Both studies are exploratory. Never present their findings as statistically conclusive.

### Two modes

- **Mode A. The participant provides a screen recording.** The recording is reviewed against the questionnaire. It adds direct evidence of actions. It does not make the study moderated, and it does not show thoughts.
- **Mode B. No recording.** The participant completes the same task and the same questionnaire. Evidence comes from their answers. Nothing about their behaviour is directly observed, so record behaviour as self-reported or Unknown.

Recording is always optional. A participant who declines or cannot record takes part fully. Their answers are used in the same way.

### The planted error

Keep the four planted-error observations separate. Do not combine them into one score.

1. **Noticed** the Thursday/Friday mismatch.
2. **Acted on it**, meaning what they say they would change, whether they opened the edit screen and whether they tried to save.
3. **Sent Sam's reply** unchanged or not, and why.
4. **Saw it** as the AI's mistake or their own misreading.

Observations 2 and 3 differ from the moderated plan, which asked whether the participant corrected the draft and was willing to authorise the corrected send. The prototype cannot show a corrected draft and cannot demonstrate a successful correction, so:
- For observation 2, record what they say they would change (self-report), whether they opened an edit screen and whether they attempted to save (recording, or self-report where there is none). A completed correction cannot be recorded. Sam's draft should never show Friday. If a recording shows it, note it as a prototype fault.
- For observation 3, record whether Sam's reply was sent unchanged and the participant's explanation. "Willing to authorise the corrected send" cannot be measured.

For observation 1, record when they noticed it, using one of these values. Each value has its own evidence source.

| Value | Meaning |
|---|---|
| While reading the draft | They report noticing it as they read the draft. |
| After seeing the edit screen | They report noticing it only after they opened the edit screen. |
| Only after re-reading | They report noticing it only after going back to the draft. |
| Reported not noticing | The participant says they did not notice it. |
| Unknown | There is not enough evidence either way. |

"Reported not noticing" and "Unknown" are different. A participant who writes nothing relevant is Unknown. Do not write "did not notice" unless the participant said so. "Confirmed not noticing" is not claimed. Nobody can confirm that someone did not notice something.

A recording can support the timing, for example showing that the participant opened Sam's edit screen before they described noticing. Record that as recording-supported. If the participant reports noticing and no recording shows when, record it as self-report only.

On the comparative study, the planted error is primary evidence only on the first exposure. Second-exposure evidence is supplementary. A later report, for example after seeing the second version, is not evidence that the participant noticed it on the first.

## Limitations of unmoderated remote testing

- There is no live observation and no neutral real-time follow-up. If a participant does something unexpected, we cannot ask why.
- Self-report can differ from what the participant actually did.
- Screen recordings improve the evidence about behaviour, but only for the people who choose to provide one. Those people may differ from the others, so the recorded group may not represent everyone.
- A screen recording cannot show every thought or intention. It shows what was on the screen.
- The prototype is a Figma mock-up, not a functioning AI system, and it has no interaction analytics. It does not take typing, so a participant who tries to type sees no change and may be confused. Record that as a prototype limit and not as a participant error. Its timers approximate real timing.
- The prototype cannot demonstrate a successful correction, so the study cannot measure whether participants correct the draft or would send a corrected one. This is a deliberate narrowing of the objective (decision 39).
- The researcher-only keyboard shortcuts (F, O and R) have been removed from both prototypes. Participants are not told about this and are not asked to avoid the keyboard. The project owner checked both prototypes in the Figma viewer on 2026-11-12 and reported no problems. Figma's own viewer may still have built-in shortcuts that cannot be removed.
- Five or six people can show patterns and usability problems. They cannot establish a statistically reliable effect.

## Running the studies

This section is for the researcher only. Do not copy anything from it into participant-facing text. The prototypes are mock-ups and send nothing. The prototype links are in [comparative-study/README.md](comparative-study/README.md#prototypes).

### Codes, order and setup

Prepare the codes before you recruit. Give each person the next unused code when they agree to take part, and keep a list of which code went to whom, apart from their answers. The code fixes the order. Never choose the order for a particular person. If a participant drops out or does not finish, replace them in the same slot so the order stays balanced.

- **General study:** P1 to P5. Every participant sees Version A only, so there is no order.
- **Comparative study:** P1 to P6, using the table below. The order is defined in the [comparative study README](comparative-study/README.md#design). Build two copies of the questionnaire named neutrally, "Form 1" and "Form 2" (see [online-questionnaire.md](online-questionnaire.md)). Keep this table on your own sheet and never show it to participants.

| Code | Form | Version 1 | Version 2 | Recording provided | Both versions completed |
|---|---|---|---|---|---|
| P1 | Form 1 | A | B | | |
| P2 | Form 2 | B | A | | |
| P3 | Form 1 | A | B | | |
| P4 | Form 2 | B | A | | |
| P5 | Form 1 | A | B | | |
| P6 | Form 2 | B | A | | |

Participants see "Version 1" and "Version 2" only. Never use A, B, old, new, original, updated, baseline, "with labels" or "without labels" in anything a participant sees or in a message to them. Questions that compare the versions come only at the end, after both versions' questions are submitted. Send each participant the matching [instructions](participant-materials/), the information page and the right links.

### Before the first participant

1. In a private browser window with no Figma login, play each prototype from screen 01: "Not now" and "Request access again", Stop at sorting and at drafting with "Resume work", an edit and Save, sending Sam then Lena (and the reverse), and the summary in each state.
2. Check that the screens move on as in the table below and that nothing resets. For the comparative study, also check that A and B differ only by the labels and the 23 px results height, and that neither leads to a screen of the other.
3. Write down anything that does not work and fix it before testing. The screen connections were read back from Figma, and the project owner checked both prototypes in the Figma viewer on 2026-11-12 and reported no problems.

| Screen | Moves on after | Goes to |
|---|---|---|
| Plan | 5 seconds | Sorting |
| Sorting | 10 seconds | Drafting |
| Drafting | 10 seconds | Results |
| "Stop requested" (before the last stage) | 3 seconds | Paused |
| "Stop requested" (last stage) | 3 seconds | Results |
| After "Not now" | 5 seconds, or sooner with "Back to task now" | The task screen |
| Paused, results, summary, edit and send screens | Never | Waits for the participant |

The instructions say only that some screens may move on by themselves. Do not tell participants about the timers or the Stop window.

Known quirks, not faults: the activity log times are fixed text. The screen behind the access pop-up is the same whichever screen opened it. Saving on any edit screen returns to the results with the text unchanged and logs nothing. Escape may not work inside the send dialogs in every Figma player, and Cancel always does. Keyboard focus starting on Cancel (decision 30) is a design rule that Figma cannot show.

### Keyboard

- The researcher-only keys F, O and R were removed from both prototypes (decision 39), so typing does nothing. Participants are told nothing about the keyboard. To reset, reopen the link.
- Escape stays and only closes the two send dialogs. It sends nothing.
- Figma's own viewer may have shortcuts that cannot be removed. If a recording shows an unexpected restart, record it as platform behaviour.

### Support messages

Reply only about technical problems, briefly and neutrally. Never confirm whether something is right, never explain how the prototype should work and never mention the planted error, dates, labels, the differences between versions or what you hope to find. Do not hint at what to click. Note every message and reply in the evidence record, because a hint would affect the evidence.

| They say | You reply |
|---|---|
| The link does not open | Send the link again. Suggest a different browser or a private window. |
| The page is blank | Suggest refreshing once and trying again. |
| The prototype went back to the start | "That can happen. Please carry on as best you can and tell us about it in the questionnaire." |
| They cannot type in the draft | "Please carry on as you would normally and tell us what you expected in the questionnaire." |
| They ask whether something is right, or what a button or word means | "I cannot answer questions about how the prototype works. Please answer as you see it." |
| They ask what you are looking for, or what the right answer is | "There are no right or wrong answers. We are testing the design, not you." |
| Comparative: which version is the newer or better one | "I would like to hear what you think after both." |
| Comparative: they notice two prototypes and ask what is different | "Please go ahead as you would normally. We will ask about both at the end." |
| Comparative: they ask whether they can go back to Version 1 | "Please carry on with Version 2 as you would normally." |
| Comparative: they ask what the labels are, or whether there are labels | Do not answer. Say: "I cannot answer questions about how the prototypes work." |

### Reviewing a recording

Review a recording only for what the screen shows, and note the time of each important moment. If no recording was provided, do not fill in actions as observed. Use the self-report from Block A and record the source as S.

- **It can show:** which screens were visited, in what order and for how long. Whether they pressed Continue, "Not now", Stop or "Resume work". Whether they opened an edit screen, pressed Save, or opened a send dialog. Whether they sent a reply, which one and what the confirmation showed. Resets, unexpected screen changes and where they seemed stuck.
- **It cannot show:** whether they read, noticed or understood anything, or why they paused or clicked. A pause on the draft is not evidence of noticing the error.
- **Comparative study:** also note whether Version 2 was opened only after the Version 1 questions were finished, whether they went back to Version 1, and in Version B whether they appear to look at a label. That is not evidence that they read or understood it.

### After each participant

1. Fill in the [evidence record](evidence-record.md) within a day, while the details are fresh. Use two records per comparative participant. Write each finding with its source and the participant's exact words.
2. Keep your interpretation in its own field and list any evidence that is missing.
3. Record familiarity with conversational AI once, and whether each participant provided a recording. Compare recorded and unrecorded participants, because the people who record may differ.

## After the data is in

1. Score nothing until the form is closed. Score the knowledge check with the answer key in the [findings template](comparative-study/comparison-and-findings-template.md). The key is for the researcher only.
2. For each important finding, write the value, the source and how sure you are. Mark patterns seen in two or more participants.
3. Do not read a failure to notice the error as evidence of excessive trust. There are other explanations, such as not reading the draft closely or not seeing a reason to check it.
4. Comparative study: after the sixth participant, complete the findings template. Compare first exposures first. Read second-exposure results as affected by learning and questionnaire priming.
5. Keep the findings of the two studies separate. Treat the results as questions for the next round. Five or six people do not give proof.

## Decisions before recruiting

**Decided (consent, privacy and data)**
- Who runs it: an individual researcher, as a personal portfolio project. Not run for an employer or company.
- Identity: participants are identified by a code only. No names or email addresses in the questionnaire. The researcher keeps the list of which code went to whom, apart from the answers.
- Form tool: Tally. No sign-in for participants. Check the tool's settings before sending (see the form configuration check in [online-questionnaire.md](online-questionnaire.md)).
- Recording route: a private upload link given with the invitation. Files are named with the participant code and Version 1 or Version 2, never a name. Recordings are kept apart from the answers.
- Storage: answers in Tally. Recordings in a private online folder that only the researcher can open.
- Retention: recordings are deleted once analysed, and no later than 90 days after the study ends. Anonymised answers and notes may be kept.
- Deletion requests: by email to the contact address, with the participant code, until the results have been written up.
- Use of results: findings and short anonymised quotes in a portfolio write-up. Recordings are never shown or shared.
- Consent: one box set for taking part, plus a separate optional box for recording. Recording is optional and does not affect whether answers are used.

**Decided (study design)**
- The research objective is narrowed to error awareness and sending decisions, with no click-based correction (decision 39).
- The researcher-only keys F, O and R were removed from both prototypes. The project owner checked both prototypes in the Figma viewer on 2026-11-12 and reported no problems.
- The knowledge check and the 1 to 5 ratings stay in both questionnaires. The knowledge check is reported understanding, not observed behaviour.
- The participant instructions do not mention the keyboard.
- Recording stays optional. Participant codes and the comparative order allocation are prepared in advance.

**Still to do before recruiting**
- [ ] The contact address. `[CONTACT ADDRESS]` appears in the information page and must be replaced.
- [ ] Which recording tools to recommend, and their steps, tested on real devices. `[DECISION]` in the information page.
- [ ] Name the private storage service and check that its upload link lets participants add files without seeing others' files.
- [ ] How to handle a recording that shows something private by accident.
- [ ] Check the consent wording and the data-handling statements against what your tools actually do. They were drafted from your choices and have not been reviewed by anyone else.
- [ ] Whether participants must be 18 or over, and how that is stated.
- [ ] The time estimates in the instructions.

**Recruiting**
- [ ] Where participants come from and how you check they fit the criteria.
- [ ] Whether you offer compensation.
