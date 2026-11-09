# Brief: AI Employee First Handoff

A small portfolio prototype of a general AI employee workspace, where the AI can take many kinds of tasks. The prototype has one short scripted scene: inbox triage. Everything is fictional and simulated. A "Simulation" label stays visible on every screen.

The screens share one simple frame: a sidebar with a task list and a "New task" entry, and a top bar with the AI employee's name (Aria, fictional). Only the triage task works.

See `decisions.md` for the reasoning behind each choice.

## Problem hypothesis (unvalidated)

People who are comfortable with chat AI may hesitate to hand work to an AI employee. They are unsure what it will do on its own and how they keep control.

This is a hypothesis. It is not a finding from research.

## User

Maya runs operations at a fictional 30-person company. She uses chat AI tools. She has never handed real work to an AI employee. She uses the tool on her own, not as part of a team.

## The scene

Maya's first task: sort this week's requests, flag the urgent ones, and draft replies for her to review.

1. **Task and limits.** Maya opens the workspace and sees one suggested task. Plain lines say what the AI will read. They also say it cannot delete or change anything, spend money or share outside the company. Nothing is sent without her say-so.
   Done when: the task and all three limits are on screen in plain words, and no technical terms appear.

2. **Granting access.** A pop-up over the workspace asks to read one fictional inbox and one board. Maya picks "Grant access" or "Not now".
   Done when: the pop-up names the inbox and board. "Not now" closes it and nothing starts. After she grants access, both names stay visible on every later screen.

3. **The plan.** A short plan appears in plain words and lists the stages ahead.
   Done when: the plan shows before any work starts, and work starts without Maya clicking anything.

4. **The AI works in stages.** A stage list is always visible with the current stage marked. A short activity log adds a line each time the AI does something. There are three stages: read, sort and flag, draft.
   Done when: the log gains a plain-language line for each stage, and the marked stage changes as the work moves on.

5. **Stop.** A Stop button is available while the AI works. After Maya presses it, the screen says "Stop requested. It will take effect at the next checkpoint, so it may not be instant." Maya can then press Continue.
   Done when: pressing Stop shows that message at once, the work halts at the next checkpoint and not before, and the log records both the request and the halt.

6. **Results and drafts.** Maya sees the sorted, ranked requests and the draft replies. Each draft is marked "Not sent". There are at least four drafts, two of them sendable.
   Done when: every draft shows "Not sent", and the requests appear in a ranked order with the urgent ones flagged.

7. **The flawed draft.** One draft has a small mistake. It says Thursday where the request said Friday.
   Done when: the wrong day is in the draft, and nothing on screen highlights it or warns about it.

8. **Editing.** Maya can open any draft and change the text.
   Done when: a saved edit changes the text, the draft still shows "Not sent", and the log has a line for the edit.

9. **Sending.** A plain "Send" option sits beside the sendable drafts. It is visible and labelled, but not highlighted, and the AI does not prompt her. When she picks it, a statement says: "This goes to someone other than you and may not be undone." The recipient is a fictional colleague, for example "Sam Okafor". She chooses Authorise or Cancel.
   Done when: the statement shows before anything is sent. Authorise sends that one message only, as a simulation. The log records it. No undo is shown. Sending a second message needs a new Authorise.

10. **Closing summary.** A short summary says what the AI did, what it did not do, and what Maya still controls.
    Done when: every action in the summary also appears in the log, and it claims nothing the simulation did not do.

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
- Logins, databases, teams or admin use.
- A permissions dashboard or extra confirmation screens.
- The AI earning more freedom over time.
- Any task other than inbox triage. "New task" and other tasks in the sidebar are not built.
- Helping users find a task. The task is suggested for them.
- In-app tracking or analytics.

## What we want to observe (written debrief)

A short written note after each session. No tracking in the app. Record these separately:

1. Did Maya notice the Thursday/Friday error?
2. Did she correct it?
3. Was she willing to authorise the corrected send, and why?

Also record:
- Did she reach the send step on her own?
- If she used Stop, how did she react to the "next checkpoint" wording?
