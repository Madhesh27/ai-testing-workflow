# Test plan – Ticket #12345 – Report export fails for large date ranges (sample)

**Goal:** Exporting the Activity report should work for any date range.
**Environment:** test.example-app.com  ·  **Account:** qa-tester@example.com

1. [AI] [read-only] Report loads for the last 7 days
   Steps: Open Reports → Activity → choose "Last 7 days"
   Expected: Table loads with no errors.

2. [AI] [read-only] Export for the last 7 days
   Steps: Same view → click Export → CSV
   Expected: File downloads.

3. [AI] [read-only] Export for the last 12 months (reported issue)
   Steps: Choose "Last 12 months" → click Export → CSV
   Expected: File downloads within 30 s.

4. [AI] [read-only] Edge case: double-click Export
   Steps: Choose "Last 7 days" → double-click Export
   Expected: One request and one file.

5. [Manual: needs a second login with a limited role] [needs 2nd user] Export as a limited-role user
   Expected: Export works, or the button is hidden if the role has no permission.

6. [Manual: needs a mobile device] Export on the mobile app
   Expected: File downloads or a share sheet opens.
