# AI Testing – run prompt

Paste this to your AI agent together with the test plan.

```
AI testing – run this test plan now on <TEST environment URL> using my logged-in TEST account.

Rules:
- Run only scenarios marked [AI]. List scenarios marked [Manual] under
  "Manual effort needed" with the reason, and do not attempt them.
- Run read-only scenarios first.
- Ask me before any step that creates or deletes data.
- Never open or change customer or production data.
- Skip "needs 2nd user" scenarios unless I give a second login.
- Result per scenario: Pass / Fail / Blocked (with reason).
- For each scenario capture: screenshot, API status codes, console errors.
- Write the ticket note ONLY from what was actually tested.
  Mark untested parts "Manual testing pending".
- Do not post to the ticketing tool, Jira or Slack without my explicit OK.
- Delete all test data you created at the end, or list what could not be deleted.

At the end give:
1. A pass/fail table per ticket
2. A ticket-ready note per ticket
3. Defect drafts (summary, steps, expected, actual, severity, priority, environment)
4. A short Slack status update
```
