# Brief: AI Employee First Handoff

A small portfolio project: an interactive Figma prototype of a general AI employee workspace, where the AI can take many kinds of tasks. The prototype has one short scripted scene: inbox triage. It will be tested in two studies: a general usability test with five people and an exploratory comparison of two versions with six people. A coded prototype is on hold until those results have been reviewed. Everything is fictional and simulated. A "Simulation" label stays visible on every screen.

The screens share one simple frame: a sidebar with a task list and a "New task" entry and a top bar with the AI employee's name (Aria, fictional). Only the triage task works. The "New task" entry is disabled and labelled "Not available in this prototype".

See `decisions.md` for the reasoning behind each choice.

## Problem hypothesis (unvalidated)

People who are comfortable with chat AI may hesitate to hand work to an AI employee. They are unsure what it will do on its own and how they keep control.

This is a hypothesis. It is not a finding from research.

## User

Maya runs operations at a fictional 30-person company. She uses chat AI tools. She has never handed real work to an AI employee. She uses the tool on her own, not as part of a team.

## The scene

Maya's first task: sort this week's requests, flag the urgent ones and draft replies for her to review.

1. **Task and limits.** Maya opens the workspace and sees one suggested task. Plain lines say what the AI will read. They also say it cannot delete or change anything, spend money or share outside the company. Nothing is sent without her approval.
   Done when: the task, all three limits and the line "Nothing is sent without your approval." are on screen in plain words and no technical terms appear.

2. **Granting access.** A pop-up over the workspace asks to read one fictional inbox and one board.
   *Normal path.* On the first task screen, Maya presses "Continue". The pop-up opens, names the inbox and board and offers "Grant access" or "Not now". If she grants access, the flow continues and both names stay visible on every later screen.
   Done when: the pop-up names the inbox and board and nothing is granted until she chooses "Grant access".
   *After "Not now".* The pop-up stays for about 5 seconds, counts down on screen and shows that nothing was granted (the requested items are struck through). A "Back to task now" link lets her return sooner. Then it closes and returns Maya to the task screen, which keeps showing that access was denied: a banner and a status chip. Its button now reads "Request access again" instead of "Continue". Pressing it opens the same pop-up, asking for the same two sources. If she chooses "Not now" again, these steps repeat. If she grants access, the flow continues.
   Done when: nothing is read or started, returning does not send another access request and nothing is granted automatically.

3. **The plan.** A short plan appears in plain words and lists the stages ahead. It says drafts are written for selected requests and it does not promise a reply for every request.
   Done when: the plan shows before any work starts and work starts without Maya clicking anything.

4. **The AI works in stages.** A stage list is always visible with the current stage marked. A short activity log adds a line each time the AI does something. There are three stages: read, sort and flag, draft.
   Done when: the log gains a plain-language line for each stage and the marked stage changes as the work moves on.

5. **Stop.** A Stop button is available while the AI works. After Maya presses it, the screen says "Stop requested. It will take effect at the next checkpoint, so it may not be instant."
   *Earlier stages (the read stage and the sort and flag stage).* The work pauses at the next checkpoint, which is the end of the stage in progress. The paused screen says where it paused and explains: "Work will resume from the next stage. Completed steps will not be repeated." Maya presses "Resume work" on that screen. It leads to the next drafting-stage screen and nothing already done is repeated.
   *Last stage (draft).* Exception: the work finishes that stage, the results appear, nothing is sent and there is no "Resume work" button. The screen says so.
   Done when: pressing Stop shows that message at once, the work halts at the next checkpoint and not before and the log records both the request and the halt. After "Resume work", the log continues from the next stage with no repeated lines. In the last stage, the log records the request and that it took effect after the drafts were written.

6. **Results and drafts.** Maya can inspect all 12 requests, ranked by urgency, with the urgent ones flagged. The AI wrote drafts for four selected requests, not for every request. The list marks which four with "Draft ready". A draft is written only when the request asks Maya a direct question that a short written reply would settle. The other requests report a problem, give a task, share an update or offer feedback, so they get no draft. Once a reply is sent, its marker changes to "Sent". Each draft is marked "Not sent" until then. Only two of the four drafts can be sent: the replies to Lena Brandt and Sam Okafor. Each one answers its request with a direct reply. Lena's says the Q3 expense report has been received and will be reviewed by the end of the week. Sam's confirms the office move walkthrough at 10:00 and says a calendar invite will follow. The other two cannot be sent here: Tomasz's says the budget must be checked first and Ava's proposes talking next week.
   Done when: all 12 requests appear in ranked order with the urgent ones flagged and the four with drafts marked, every draft shows "Not sent", the screen says which two drafts can be sent and nothing implies that every request has a draft.

7. **The flawed draft.** One draft has a small mistake. It says Thursday where the request said Friday.
   Done when: the wrong day is in the draft and nothing on screen highlights it or warns about it. Until Maya edits it, every place the draft appears says Thursday, including the send confirmation and the sent card if she sends it unedited.

8. **Editing.** Maya can open any draft and change the text. Saving returns her to the results. Cancel returns her there and leaves the draft unchanged.
   Done when: a saved edit changes the text, the draft still shows "Not sent" and the log has a line for the edit. If she corrects Sam's draft, it says Friday everywhere it appears afterwards: the results, the send confirmation and the sent card.

9. **Sending.** A plain "Send" option sits beside the sendable drafts. It is visible and labelled, but not highlighted and the AI does not prompt her. When she picks it, a statement says: "This goes to someone other than you and may not be undone." The recipient is a fictional colleague, for example "Sam Okafor". She chooses Authorise or Cancel, which have equal visual weight. She can send a draft with or without editing it first. If she sends Sam's original draft unedited, the confirmation shows the text as it stands, with Thursday and no warning. The sent card shows the same text.
   Done when: the statement shows before anything is sent. Authorise sends that one message only, as a simulation. The log records it. No undo is shown. A sent draft is locked: it cannot be edited or sent again. Sending a second message needs its own Authorise and its dialog says the earlier approval does not carry over.

10. **Closing summary.** Maya starts it herself with "Finish and view summary", available once the results are shown, whether or not she sent anything. A short summary says what the AI did. It does not repeat the limits or list what Maya still controls. It reads correctly if no message, one message or two messages were sent. It is not available while the work is paused and becomes available after the work finishes. After a stop in the last stage, the summary says that Maya asked to stop, that the drafts were finished first and what was sent. After an earlier stop, it records the pause, Maya's decision to resume and the final outcome. It never reads like an uninterrupted run.
    Done when: every action in the summary also appears in the log and it claims nothing the simulation did not do.

## Words we use

- **"Continue" on the first task screen** starts the access request. It opens the pop-up.
- **"Request access again"** replaces that button after "Not now". It opens the same pop-up.
- **"Resume work"** on the paused screen resumes the work from the next stage.

## What the AI may do

**Alone:**
- Read the inbox and board Maya granted.
- Sort, rank and summarise requests.
- Write draft replies that only Maya can see.

**Only with Maya's approval:**
- Send a message to someone other than Maya. Each send needs its own approval.

**Never:**
- Delete or change existing items.
- Spend money.
- Share anything outside the company.

## Out of scope

- Real AI, real email or any real connection.
- A coded prototype. It is on hold until the Figma prototype has been tested.
- Logins, databases, teams or admin use.
- A permissions dashboard or extra confirmation screens.
- The AI earning more freedom over time.
- Any task other than inbox triage. "New task" and other tasks in the sidebar are not built.
- Helping users find a task. The task is suggested for them.
- In-app tracking or analytics.

## What we want to observe (written debrief)

Two remote, unmoderated studies use the Figma prototype: a general usability test with five people and a comparison of two versions with six people. Participants work alone, answer an online questionnaire and may choose to send a screen recording. The procedure, the evidence rules and the limitations are in [usability-test/test-plan.md](../usability-test/test-plan.md). In the comparison, each person sees both versions and all four planted-error observations below count only on their first version. Record these separately:

1. Did Maya notice the Thursday/Friday error?
2. Did she act on it?
3. Was she willing to authorise the corrected send and why?
4. If Maya notices the planted error, does she see it as the AI's mistake or her own misreading?

The prototype cannot demonstrate a successful correction. Item 2 is recorded as what the participant says they would change, whether they opened the edit screen and whether they attempted to save. Item 3 is recorded as whether Sam's reply was sent unchanged, and the participant's explanation. A failure to notice the error is not read as evidence of excessive trust.

Also record:
- Did she reach the send step on her own?
- If she used Stop, how did she react to the "next checkpoint" wording?
- After editing, did she understand the draft was still private?
- If she chose "Not now", did she understand that nothing had been granted or started and how did she react to the countdown, the denied-access status and the "Request access again" button?
