# Decisions

One line each: the choice, then why.

1. **Safe delegation leads.** Handing over responsibility is what makes an AI employee different from a chatbot.
2. **The user is an AI-literate first-time delegator, using it alone.** Teams and admin use add problems that a small prototype cannot test.
3. **The product is a general AI employee workspace. The prototype tests one scene in it: Maya's inbox triage.** The workspace shows that the AI can take many kinds of tasks, but only triage is built. Triage is a real, multi-step task and low-risk while drafts stay private.
4. **The AI acts alone only on safe things.** It reads, sorts, flags and drafts privately. Any send needs approval. It never deletes, spends money or shares outside the company. This is a simple rule to explain.
5. **One flawed draft, with no highlight and no warning.** A believable mistake (Thursday instead of Friday) tests whether Maya can judge the AI's work. We accept it may feel like a trick.
6. **Drafts are editable, and each edit is logged.** We need to see whether she corrects the error.
7. **The send is visible and labelled, but not emphasised, and the AI never nudges.** Handing over should be Maya's choice. We accept some testers may never send.
8. **Each approval covers one send only.** The first experience stays honest about control. There is no "approve similar sends".
9. **The send says it goes to someone other than Maya and may not be undone, and there is no fake undo.** False comfort would damage the trust we are testing.
10. **Control means a plan, a visible log and a stop. Stop works at the next checkpoint and says so.** It is much cheaper than a stop that interrupts at once, and it is honest about how real agents behave.
11. **Front-end only, scripted data, no AI backend.** It fits a small portfolio scope.
12. **Reactions are captured in a short written debrief, with no in-app tracking.** Notes fit the hypothesis. We accept little numeric data.
13. **The scene ends with a closing summary.** It says what the AI did, what it did not do, and what Maya still controls. It is neutral and makes no claim about draft quality.
14. **Three visible AI stages (read, sort and flag, draft), at least four drafts, at least two sendable.** A second send can only be tested if there are two sendable drafts.
15. **The send recipient is a fictional colleague.** The AI never shares outside the company, so the send must not contradict that.
16. **No generic "AI can make mistakes" line.** It would hint at the planted error and spoil the test.
17. **Maya can press Continue after a stop.** Otherwise an early stop ends the scene before the draft and send, and we learn nothing.

Also decided: no progressive autonomy in this prototype, because it is not needed to test the hypothesis.
