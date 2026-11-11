# Version B wireframes

Version B is the comparison version in the [comparative study](../../usability-test/comparative-study/README.md). Version A is the existing set of screens in [design/version-a/](../version-a/), unchanged.

Version B adds one thing: short authority labels at the point of action. The scenario, the requests, the drafts, the planted error and the interactions are unchanged. The only other difference is a small layout change that the labels cause, described below. All names, companies and messages are fictional.

This folder holds only the screens that differ from Version A. Every other screen is the same as in Version A.

## The labels

The labels are muted text in the same style as existing hint text, in fixed positions. They are not buttons and they do not draw attention to Send.

| Where | Label |
|---|---|
| Plan, step 1 | Read-only access |
| Plan, step 2 | No changes to requests |
| Plan, step 3 | Drafts remain private |
| Sorting screens | No changes to requests |
| Drafting screens | Drafts remain private |
| Lena's and Sam's draft cards, next to Send | Approval required to send |

"No changes to requests" means the original requests are not modified. Sorting and ranking still happen. "Approval required to send" shows only while a card's Send button is available.

## Screens that differ

Overview of all 26 Version B screens, including the 11 that are identical to Version A: [overview-b.png](overview-b.png)

| Screen | Version B | Version A |
|---|---|---|
| 3. The plan | [04-plan.png](04-plan.png) | [04-plan.png](../version-a/04-plan.png) |
| 4. Sorting | [05-working.png](05-working.png) | [05-working.png](../version-a/05-working.png) |
| 4. Writing the drafts | [05b-working-write-drafts.png](05b-working-write-drafts.png) | [05b-working-write-drafts.png](../version-a/05b-working-write-drafts.png) |
| 5. Stop requested | [06-stop-requested.png](06-stop-requested.png) | [06-stop-requested.png](../version-a/06-stop-requested.png) |
| 5. Writing the drafts after Resume work | [07b-working-write-drafts-after-resume.png](07b-working-write-drafts-after-resume.png) | [07b-working-write-drafts-after-resume.png](../version-a/07b-working-write-drafts-after-resume.png) |
| 5. Stop requested in the last stage | [08-stop-in-last-stage.png](08-stop-in-last-stage.png) | [08-stop-in-last-stage.png](../version-a/08-stop-in-last-stage.png) |
| 5. Results after a stop in the last stage | [09-results-after-last-stage-stop.png](09-results-after-last-stage-stop.png) | [09-results-after-last-stage-stop.png](../version-a/09-results-after-last-stage-stop.png) |
| 6 and 7. Results and drafts | [10-results-and-drafts.png](10-results-and-drafts.png) | [10-results-and-drafts.png](../version-a/10-results-and-drafts.png) |
| 8. Results after saving an edit | [10b-results-after-saving-an-edit.png](10b-results-after-saving-an-edit.png) | [10b-results-after-saving-an-edit.png](../version-a/10b-results-after-saving-an-edit.png) |
| 9. Authorise one send | [12-authorise-send.png](12-authorise-send.png) | [12-authorise-send.png](../version-a/12-authorise-send.png) |
| 9. Authorise one send, Sam's original draft | [12b-authorise-send-original-draft.png](12b-authorise-send-original-draft.png) | [12b-authorise-send-original-draft.png](../version-a/12b-authorise-send-original-draft.png) |
| 9. After sending (simulated) | [13-sent.png](13-sent.png) | [13-sent.png](../version-a/13-sent.png) |
| 9. After sending Sam's original draft (simulated) | [13b-sent-original-draft.png](13b-sent-original-draft.png) | [13b-sent-original-draft.png](../version-a/13b-sent-original-draft.png) |
| 9. Authorise a second send | [14-authorise-second-send.png](14-authorise-second-send.png) | [14-authorise-second-send.png](../version-a/14-authorise-second-send.png) |
| 9. After the second send (simulated) | [15-both-sent.png](15-both-sent.png) | [15-both-sent.png](../version-a/15-both-sent.png) |

## One layout consequence of the labels

On the results screens, Lena's and Sam's cards each gain one muted line ("Approval required to send"), in the same position as the existing "Sending is not available for this draft." line on the other two cards. That is a height increase of one line, about 23 px. The results screens are 1253 px tall in Version B and 1230 px in Version A, and the content below the top row of cards moves down by the same amount. Nothing else on those screens changes.

The other screens, including the first screen, the access pop-up, the edit screens and the summaries, are unchanged. They are in [design/version-a/](../version-a/).
