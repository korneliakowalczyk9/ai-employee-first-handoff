# Facilitator guide

How to run a session with the interactive Figma prototype. Read this with [test-plan.md](test-plan.md). Record each session with [observation-template.md](observation-template.md).

The prototype is a mock-up. It is not a real AI employee, and nothing in it is sent. The prototype link is shared by the project owner and is not stored in this repository.

## Before the first session: play it through once

The connections between screens were checked by reading them back from Figma. The timers, key presses and conditional logic have not been run, so play the prototype yourself before any participant does.

1. Present from screen 01. Check Continue, Grant access and the wait to the plan.
2. Let it run through sorting, drafting and the results, about 25 seconds.
3. Press **R**. Stop at sorting, then check the paused screen, "Resume work", the results and the summary wording.
4. Press **R**. Stop at drafting and check the results and the summary wording.
5. On the results, scroll down. Open Sam's edit screen, press **F**, save, and check that Friday and the log line appear. Press **R** and try **O**.
6. Send Sam. Check the preview, Escape and Cancel, then Authorise and the locked card.
7. Send Lena and check the line that says the earlier approval does not carry over. Try the reverse order.
8. Open the summary in each state. Press **R** to check the reset.
9. Write down anything that does not work and fix it before testing.

## Before each session

1. Open the Figma file, go to the page "Prototype", select "01 Task and limits" and press Present.
2. Check the prototype is at 100 percent and fits the screen without browser bars covering it.
3. Press **R** once. This resets everything to the start state.
4. Keep the observation template open. Keep this guide out of the participant's view.
5. Press **R** again, so the participant starts from screen 01.

## What moves on its own

| Screen | Moves on after | Goes to |
|---|---|---|
| Plan | 5 seconds | Sorting |
| Sorting | 10 seconds | Drafting |
| Drafting | 10 seconds | Results |
| "Stop requested" (before the last stage) | 3 seconds | Paused |
| "Stop requested" (last stage) | 3 seconds | Results |
| After "Not now" | 5 seconds, or sooner with "Back to task now" | The task screen |
| Paused, results, summary and the edit and send screens | Never | Waits for the participant |

Sorting and drafting each last 10 seconds, so the participant has time to press Stop. Do not mention this.

## Facilitator keys

These keys are invisible. Nothing on screen tells the participant they exist. Press them only as described below.

| Key | Works on | What it does |
|---|---|---|
| **F** | Results, Sam's edit screen, Sam's send dialog | Shows the date corrected: Sam's draft says Friday and the log records "You edited the draft reply to Sam Okafor." Ignored once Sam's reply has been sent. |
| **O** | The same three screens | Shows an edit that is not the date: the draft stays as it is and nothing is logged. Also undoes an accidental F. Ignored once Sam's reply has been sent. |
| **R** | Every screen | Resets all state and returns to screen 01. On screen 01 it only resets. |
| **Esc** | Both send dialogs | Closes the dialog and sends nothing. The participant may use it too. |

The edit box on Sam's edit screen updates to match whichever key you press.

## The editing step

The prototype cannot take free typing, so you control what the edit shows.

1. Do nothing until the participant opens an edit screen on their own.
2. When they do, say only: "Please tell me out loud what you would change, and I will show you the result."
3. Listen. Write down exactly what they say.
4. If they say they would change the date to Friday, press **F**.
5. If they describe any other change, or nothing, press **O**. Do not suggest anything else.
6. They press Save. They see the results.
7. If they press Save before you have pressed a key, press the key on the results screen. It updates the draft there.

Never say or do anything that points at the date or the word Thursday or Friday. Never suggest that the draft needs a correction. If the participant never opens an edit screen, do not offer one.

## Sending

- If the participant sends Sam's reply without editing it, say nothing. The dialog and the sent card will show the original text.
- If the participant asks whether they should send, say: "What would you do if this were real?"
- Each send has its own dialog. Do not explain it.

## What to do when the participant

| Situation | You do |
|---|---|
| Asks "Is this right?" or "Did it do it correctly?" | "What would you do if this were real?" |
| Asks what a button does | "What do you expect it to do?" |
| Goes quiet for more than about 20 seconds | "What are you thinking?" |
| Presses Stop | Say nothing. Note what they say about the wording. |
| Chooses "Not now" | Say nothing. Note their reaction to the countdown and the status. |
| Asks to go back | Say "Go ahead as you would normally." If the prototype cannot go back, note it. |
| Reaches the summary | Let them read it. Do not prompt. |
| Seems stuck or the prototype breaks | Note the screen and what happened. Press **R** if you must restart. Say: "Let's pick it up from the start of that part." |

## Rules

- Never reveal or hint at the planted error.
- Never suggest sending or not sending, or editing or not editing.
- Never praise or criticise what the participant does.
- Do not explain screens. Ask what they expect.
- Only the participant decides what to do. The keys follow what they say.

## Known limits of the prototype

- The timers are approximate. The plan, working and Not now screens move on by themselves after a few seconds.
- The activity log times are fixed text.
- The screen behind the access pop-up is the same whichever screen opened it.
- Only the date correction can be shown as an edit. Other edits are noted, not shown.
- Only Sam's edit screen responds to the F and O keys. Saving on the other drafts' edit screens returns to the results with the text unchanged and nothing logged. Note what the participant said.
- Keyboard focus starting on Cancel in the send dialogs (decision 30) is a design rule that Figma cannot show. It is described in `design/README.md`.
- Keys F and O are single letters. If the participant types into any field, a stray F or O can trigger them. Ask the participant not to use the keyboard if this happens.
- Pressing F or O after a send does not change the log order. Press them before sending.
- Escape and R may not work inside the send dialogs in every Figma player. If Escape does not work, the participant can use Cancel.

## After each session

1. Press **R**.
2. Fill in the observation template within an hour.
3. Note any point where your words or keys may have helped the participant, in "Facilitator conduct".
