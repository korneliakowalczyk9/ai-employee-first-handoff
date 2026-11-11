# Wireframes

Low-fidelity screens for the inbox triage scene, in step order. All names, companies and messages are fictional.

## Two versions

| Folder | Version | What it is |
|---|---|---|
| [version-a/](version-a/README.md) | A | The approved wireframes, with no point-of-action labels. All 26 screens. |
| [version-b/](version-b/README.md) | B | The same screens with short authority labels added. Only the 15 screens that differ. |

The two versions are compared in an exploratory [comparative study](../usability-test/comparative-study/README.md). The table below lists the Version A screens. The interaction notes after it apply to both versions.

## Version A screens

| Step | Screen |
|---|---|
| All | [00-overview.png](version-a/00-overview.png) (all 26 screens on one page) |
| 1. Task and limits | [01-task-and-limits.png](version-a/01-task-and-limits.png) |
| 2. Granting access (pop-up) | [02-access-popup.png](version-a/02-access-popup.png) |
| 2. Access pop-up after Not now | [03-access-popup-after-not-now.png](version-a/03-access-popup-after-not-now.png) |
| 2. Task screen after Not now | [01b-task-and-limits-after-not-now.png](version-a/01b-task-and-limits-after-not-now.png) |
| 3. The plan | [04-plan.png](version-a/04-plan.png) |
| 4. The AI works in stages | [05-working.png](version-a/05-working.png) |
| 4. The AI writes the drafts | [05b-working-write-drafts.png](version-a/05b-working-write-drafts.png) |
| 5. Stop requested | [06-stop-requested.png](version-a/06-stop-requested.png) |
| 5. Paused, Resume work available | [07-paused.png](version-a/07-paused.png) |
| 5. Writing the drafts after Resume work | [07b-working-write-drafts-after-resume.png](version-a/07b-working-write-drafts-after-resume.png) |
| 5. Stop requested in the last stage | [08-stop-in-last-stage.png](version-a/08-stop-in-last-stage.png) |
| 5. Results after a stop in the last stage | [09-results-after-last-stage-stop.png](version-a/09-results-after-last-stage-stop.png) |
| 6 and 7. Results and drafts | [10-results-and-drafts.png](version-a/10-results-and-drafts.png) |
| 8. Results after saving an edit | [10b-results-after-saving-an-edit.png](version-a/10b-results-after-saving-an-edit.png) |
| 8. Editing a draft | [11-edit-a-draft.png](version-a/11-edit-a-draft.png) |
| 9. Authorise one send | [12-authorise-send.png](version-a/12-authorise-send.png) |
| 9. Authorise one send, Sam's original draft | [12b-authorise-send-original-draft.png](version-a/12b-authorise-send-original-draft.png) |
| 9. After sending (simulated) | [13-sent.png](version-a/13-sent.png) |
| 9. After sending Sam's original draft (simulated) | [13b-sent-original-draft.png](version-a/13b-sent-original-draft.png) |
| 9. Authorise a second send | [14-authorise-second-send.png](version-a/14-authorise-second-send.png) |
| 9. After the second send (simulated) | [15-both-sent.png](version-a/15-both-sent.png) |
| 10. Summary, no messages sent | [16-summary-no-messages-sent.png](version-a/16-summary-no-messages-sent.png) |
| 10. Summary, after a stop in the last stage | [16b-summary-after-last-stage-stop.png](version-a/16b-summary-after-last-stage-stop.png) |
| 10. Summary, after a stop before the last stage | [16c-summary-after-earlier-stop.png](version-a/16c-summary-after-earlier-stop.png) |
| 10. Summary, one message sent | [17-summary-one-message-sent.png](version-a/17-summary-one-message-sent.png) |
| 10. Summary, two messages sent | [18-summary-two-messages-sent.png](version-a/18-summary-two-messages-sent.png) |

The access pop-up (screen 02) is one shared dialog. It opens from the first task screen (01) and from the task screen after "Not now" (01b). When it opens from 01b, the task screen behind it keeps the "Access not granted" banner, the status chip and the "Request access again" button. The dimmed background in the frame for screen 02 is illustrative only.

## Interaction notes

The images are static, so the behaviour between screens is described here. The reasoning is in [docs/decisions.md](../docs/decisions.md).

**Access**
- "Continue" on screen 01 opens the access pop-up (02).
- "Not now" shows screen 03 for about 5 seconds, with the countdown "Returning to the task screen in 5 seconds…". "Back to task now" returns sooner. Either way Maya lands on screen 01b.
- Returning never sends an access request. Nothing is granted automatically.
- "Request access again" on 01b opens the same pop-up (02), asking for the same two sources with nothing pre-selected. "Not now" repeats the steps above and "Grant access" continues to the plan (04).

**Work, Stop and Resume work**
- The work starts by itself after the plan appears and Maya does not click anything.
- Stop before the last stage (screens 05 to 07): the work pauses at the next checkpoint, which is the end of the stage in progress. The paused screen (07) says where it paused.
- "Resume work" on the paused screen leads to the drafting screen (07b). It resumes from the next stage and repeats nothing already done. The paused screen explains this: "Work will resume from the next stage. Completed steps will not be repeated."
- Without a stop, the work moves from screen 05 to the drafting screen (05b) and then to the results (10).
- Stop in the last stage (screen 08): the work finishes the drafts, the results appear (09) and nothing is sent. There is no "Resume work" button.

**Results and editing**
- The results show all 12 ranked requests with the urgent ones flagged. Four of them have drafts and the list marks which four. No screen implies that every request has a draft.
- Only the replies to Lena and Sam have a Send button.
- "Save" on the edit screen (11) returns to the results (10b). The edited draft shows her text and is still marked "Not sent". The log adds "You edited the draft reply to …". "Cancel" returns to the results and leaves the draft unchanged.
- Sam's original draft says Thursday. After Maya corrects and saves it, it says Friday everywhere it appears: the results, the send confirmation and the sent card.

**Sending**
- When a send confirmation opens (12 and 14), keyboard focus starts on Cancel. Escape cancels and nothing is sent unless Maya chooses Authorise.
- Authorise sends only the reply in the dialog. Each send has its own confirmation and the second one says the earlier approval does not carry over.
- If Maya sends Sam's original draft without editing it, the confirmation (12b) shows the text as it stands, with Thursday and no warning. The sent card (13b) shows the same text.
- A sent draft shows "Sent (simulated)" and loses its Edit and Send buttons. It cannot be edited or sent again.

**Summary**
- "Finish and view summary" is on the results screens and opens the summary. Which of screens 16 to 18 appears depends on how many messages were sent.
- A summary is not available while the work is paused. It becomes available after the work finishes.
- After a stop in the last stage, the summary says that Maya asked to stop, that the drafts were finished first and what was sent (screen 16b shows the case where nothing was sent). The same stop line appears in the summary when one or two messages were sent.
- After a stop before the last stage, the summary records the pause, Maya's decision to resume and the final outcome (screen 16c shows the case where nothing was sent). The same line appears when one or two messages were sent.

The steps are described in [docs/brief.md](../docs/brief.md).
