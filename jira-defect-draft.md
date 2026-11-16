# Defect draft (sample, not logged until approved)

**Summary:** Test – Reports – Activity export returns 500 for a 12-month date range

**Description:** Exporting the Activity report works for short ranges but fails for the last 12 months. The export API returns 500 after about 7 seconds and no file is downloaded.

**Environment:** test.example-app.com, Chrome, test account

**Steps to reproduce**
1. Open Reports → Activity
2. Choose "Last 12 months"
3. Click Export → CSV

**Expected result:** The CSV downloads within 30 seconds.

**Actual result:** `GET /api/reports/activity/export` returns 500 after ~7 s. Console shows "Export failed: 500". No file.

**Severity:** Major · **Priority:** High

**Attachments:** S3.png, network log
