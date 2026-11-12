# Comparison and findings template

Fill this in after all six participants have submitted both versions. Do not score any participant's answers before then.

This page is for the analyst only. It contains the answer key, so never show it to participants.

Remember what the results can and cannot show: six people, one scenario, a repeated task and no live observation do not give statistical evidence. The evidence rules, sources (R, S, R+S, U) and limitations are in the [test plan](../test-plan.md#evidence) and the [README](README.md#what-the-results-can-and-cannot-tell-us). Unknown is not a failure and it is not a success.


## 1. Participants and order

| Participant | Version 1 (first) | Version 2 (second) | Recording provided (Yes / No, and for which version) | Familiarity with conversational AI (their words, from the first evidence sheet) | Notes |
|---|---|---|---|---|---|
| P1 | A | B | | | |
| P2 | B | A | | | |
| P3 | A | B | | | |
| P4 | B | A | | | |
| P5 | A | B | | | |
| P6 | B | A | | | |

Use the familiarity column to account for differences in prior AI experience when you interpret the results, for example when one order group has more experienced participants than the other. Use the recording column to check whether the participants who recorded differ from those who did not, for example in familiarity or in what they said.

## 2. Knowledge check: answer key and scoring

Score after all responses are in. One point for each correct answer. "Not sure" and blank answers score 0. This measures reported understanding, collected from the questionnaire. It is self-report, and it is not observed behaviour. Do not describe a score as something the participant did.

| # | Statement | Correct answer | Group |
|---|---|---|---|
| 1 | Read the inbox and the board you gave access to | Aria does this on its own | On its own |
| 2 | Sort the requests and flag the urgent ones | Aria does this on its own | On its own |
| 3 | Write a draft reply that only you can see | Aria does this on its own | On its own |
| 4 | Send a reply to a colleague | Aria needs my approval first | Needs approval |
| 5 | Send a second reply without asking for my approval again | Aria needs my approval first, or Aria cannot do this (see note) | Needs approval |
| 6 | Delete a request | Aria cannot do this | Cannot do |
| 7 | Spend money | Aria cannot do this | Cannot do |
| 8 | Share something outside the company | Aria cannot do this | Cannot do |

Note on statement 5: it tests whether the participant understands that approval for the first reply does not authorise a second one. The statement describes Aria sending without asking again, so a participant who understands may answer either "Aria needs my approval first" or "Aria cannot do this". Score either as correct, record which was given, and count the statement in the "Needs approval" group.

Record the score for each participant and each exposure.

| Participant | Version seen | Exposure | Total (0 to 8) | On its own (0 to 3) | Needs approval (0 to 2) | Cannot do (0 to 3) |
|---|---|---|---|---|---|---|
| P1 | | 1 | | | | |
| P1 | | 2 | | | | |
| P2 | | 1 | | | | |
| P2 | | 2 | | | | |
| P3 | | 1 | | | | |
| P3 | | 2 | | | | |
| P4 | | 1 | | | | |
| P4 | | 2 | | | | |
| P5 | | 1 | | | | |
| P5 | | 2 | | | | |
| P6 | | 1 | | | | |
| P6 | | 2 | | | | |

Also list which statements were answered wrongly most often in each version and what the wrong answers were.

Statements 6 to 8 (the things Aria cannot do) have no matching label in Version B. Use them as a rough check. If scores on them also rise in Version B, or on the second exposure, the cause may be learning, questionnaire priming or a general effect and not the labels.

## 3. Ratings (stated opinion)

Record the five ratings (C1 to C5, each 1 to 5) for each participant and each exposure, and keep them separate. First-exposure ratings are the primary evidence. Second-exposure ratings are supplementary (see the [README](README.md#primary-evidence-is-the-first-exposure)).

| Participant | Version | Exposure | C1 Allowed | C2 Approval | C3 Control | C4 Comfortable | C5 Clear steps |
|---|---|---|---|---|---|---|---|
| P1 | | 1 | | | | | |
| P1 | | 2 | | | | | |
| P2 | | 1 | | | | | |
| P2 | | 2 | | | | | |
| P3 | | 1 | | | | | |
| P3 | | 2 | | | | | |
| P4 | | 1 | | | | | |
| P4 | | 2 | | | | | |
| P5 | | 1 | | | | | |
| P5 | | 2 | | | | | |
| P6 | | 1 | | | | | |
| P6 | | 2 | | | | | |

## 4. Behaviour and evidence (first exposure, the primary evidence)

Copy from the first-exposure [evidence records](../evidence-record.md). For each cell write the value and its source. Use counts and short notes, not interpretations. A participant without a recording has S or Unknown only. Do not fill in their behaviour as if it had been observed.

| Participant | Version | Recording | Said or asked about approval | Hesitated before Send | Tried to send something not sendable | Went back or re-read | Confusion points (screen, seriousness) | Sent a reply (which) |
|---|---|---|---|---|---|---|---|---|
| P1 | | | | | | | | |
| P2 | | | | | | | | |
| P3 | | | | | | | | |
| P4 | | | | | | | | |
| P5 | | | | | | | | |
| P6 | | | | | | | | |

### The planted error (first exposure only)

Keep the four observations separate and do not combine them into one trust score. The values, sources and rules are in the [evidence record](../evidence-record.md#3-the-planted-error) and the [test plan](../test-plan.md#the-planted-error).

For observation 1 copy the value and its source from the evidence record. "Reported not noticing" and "Unknown" are different.

| Participant | Version | Recording | 1. Noticed (value and source) | 2. Acted on it (would change, opened edit, attempted save) | 3. Sent Sam's reply unchanged, and explanation | 4. Aria's mistake or own misreading |
|---|---|---|---|---|---|---|
| P1 | | | | | | |
| P2 | | | | | | |
| P3 | | | | | | |
| P4 | | | | | | |
| P5 | | | | | | |
| P6 | | | | | | |

The prototypes cannot demonstrate a successful correction, so a completed correction cannot be recorded. Observation 2 records what the participant says they would change, whether they opened the edit screen and whether they attempted to save. Observation 3 records whether Sam's reply was sent unchanged and the participant's explanation. Sam's draft should never show Friday. If it does, note a prototype fault and do not count it.

## 5. Primary comparison: first exposure, A-first against B-first

Participants 1, 3 and 5 saw A first. Participants 2, 4 and 6 saw B first. Each participant contributes one first-exposure result.

| Measure | A first (P1, P3, P5) | B first (P2, P4, P6) | Direction |
|---|---|---|---|
| Knowledge check total | list the three scores | list the three scores | |
| On its own (0 to 3) | | | |
| Needs approval (0 to 2) | | | |
| Cannot do (0 to 3) | | | |
| C1 Allowed | | | |
| C2 Approval | | | |
| C3 Control | | | |
| C4 Comfortable | | | |
| C5 Clear steps | | | |
| Behaviour: approval questions, hesitation at Send, confusion points | | | |

List the individual values. With three people per group, do not report averages as if they were precise, and do not present a simple Version 1 against Version 2 score as conclusive. Individual responses, explanations and observed behaviour matter most.

## 6. Secondary comparison: each person's A against B

This is supplementary. It is affected by order, learning and questionnaire priming (see the [README](README.md#primary-evidence-is-the-first-exposure)). Read it with the order in the table above, as support for the first-exposure comparison and not as a result on its own.

| Participant | Order | Total in A | Total in B | B minus A | C1 in A | C1 in B | C2 in A | C2 in B | C3 in A | C3 in B | C4 in A | C4 in B |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| P1 | A→B | | | | | | | | | | | |
| P2 | B→A | | | | | | | | | | | |
| P3 | A→B | | | | | | | | | | | |
| P4 | B→A | | | | | | | | | | | |
| P5 | A→B | | | | | | | | | | | |
| P6 | B→A | | | | | | | | | | | |

Count how many of the six have a higher, equal or lower knowledge-check total in B:
- Higher in B: __ of 6
- Equal: __ of 6
- Lower in B: __ of 6

### Order effect

| Participant | Order | Total, first exposure | Total, second exposure | Change |
|---|---|---|---|---|
| P1 | A→B | | | |
| P2 | B→A | | | |
| P3 | A→B | | | |
| P4 | B→A | | | |
| P5 | A→B | | | |
| P6 | B→A | | | |

If scores rise on the second exposure whichever version it is, learning or questionnaire priming is part of any difference. Say so in the findings.

## 7. Recording against self-report

Compare what the recordings show with what people said and scored. Look for mismatches. This is possible only for participants who provided a recording. For the others there is nothing to compare, so write "No recording".

| Participant | What the recording shows (R) | What they scored | What they said (S) | Mismatch? |
|---|---|---|---|---|
| P1 | | | | |
| P2 | | | | |
| P3 | | | | |
| P4 | | | | |
| P5 | | | | |
| P6 | | | | |

Examples of mismatches: rated "I understood what needs my approval" highly but answered statement 5 wrongly, or said they felt in control but hesitated and asked what Aria could do.

## 8. Comparison questions and open comments

| Participant | Which was easier to understand | Which they would use | Their reasons (own words) | What they said was different |
|---|---|---|---|---|
| P1 | | | | |
| P2 | | | | |
| P3 | | | | |
| P4 | | | | |
| P5 | | | | |
| P6 | | | | |

Group the open comments into themes. For each theme, note how many participants raised it, in which version and keep one short quote.

## 9. Does the "Approval required to send" label affect Send?

The risk is that the label makes Send more noticeable. Check only the evidence that exists. Participants without a recording give no behavioural evidence here. Write the source with each answer.

| Question | A first | B first |
|---|---|---|
| Did participants reach Send? (source) | | |
| How long did they hesitate before Send? (recording only) | | |
| Did anyone mention the label in their answers? (S) | | |
| Did anyone send sooner or more often than in the other group? (source) | | |

Do not draw a conclusion from one or two cases. Report what the evidence shows and what is Unknown.

## 10. Working rules for interpreting the results

These rules were set before any data was collected, so that the interpretation is not decided afterwards. They are not statistical tests. Even "Tentatively supported" is not evidence of a reliable effect: with six people, 5 of 6 can easily arise by chance.

| Reading | When it applies |
|---|---|
| Tentatively supported | The first-exposure groups differ in the same direction as the hypothesis and at least 5 of 6 paired differences point the same way and comments mention clarity or approval. |
| Mixed | The first-exposure groups and the paired differences disagree, or only 3 or 4 of 6 point the same way. |
| No clear difference | Scores differ by 1 point or less, or the direction is split. |
| Contrary | Version B is lower on the first exposure and in at least 5 of 6 paired differences. |

State which reading applies for each measure: knowledge check, C1 understanding of what Aria may do, C2 approval, C3 control and C4 comfort. They use the same readings and thresholds, and each rating is read separately. C5 (clarity of the workflow) is reported descriptively in sections 3 and 5 and has no reading.

First-exposure results come first. Paired differences can support a first-exposure difference but never establish one on their own.

## 11. Findings

| Measure | Reading (from section 10) | Evidence and its sources (R, S, reported understanding, U) | Confidence (low / very low) |
|---|---|---|---|
| Understanding of what Aria may do independently (knowledge check + C1) | | | |
| Understanding of what needs approval | | | |
| Feeling of control | | | |
| Comfort delegating | | | |
| Send salience | | | |

Write the findings in plain sentences, for example: "In the first exposure, two of the three participants who saw Version B answered statement 5 correctly, against one of three who saw Version A. This is consistent with the hypothesis but too few to rely on."

### What we can say

-

### What we cannot say

-

Always include the limits in the [README](README.md#weaknesses-specific-to-this-design) and the [test plan](../test-plan.md#limitations-of-unmoderated-remote-testing). Name in particular: six participants, one scenario, learning, questionnaire priming, Version B's extra text, its 23 px taller results cards, no live observation, and that behaviour is known only for participants who recorded (the others are self-reported or Unknown). The study tests the label-and-presentation treatment as implemented and does not isolate the labels alone.

### Questions for a next round

-
