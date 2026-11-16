# Run report – Ticket #12345 (sample)

**Environment:** test.example-app.com · **Account:** qa-tester@example.com · **Run by:** AI agent, reviewed by QA

| # | Scenario | Result | API | Console | Evidence |
|---|---|---|---|---|---|
| 1 | Report loads (7 days) | ✅ Pass | `GET /api/reports/activity` 200 (1.2 s) | none | S1.png |
| 2 | Export (7 days) | ✅ Pass | `GET /api/reports/activity/export` 200, 48 KB | none | S2.png |
| 3 | Export (12 months) | ❌ Fail | `GET /api/reports/activity/export` **500** after ~7 s | `Export failed: 500` | S3.png |
| 4 | Double-click Export | ✅ Pass | 1 request, 200 | none | S4.png |
| 5 | Limited-role user | ⏳ Manual pending | — | — | needs 2nd login |
| 6 | Mobile app | ⏳ Manual pending | — | — | needs device |

**Summary:** 3 Pass · 1 Fail · 2 Manual pending

**Manual effort needed**
- Scenario 5: needs a second login with a limited role.
- Scenario 6: needs a mobile device.

**Test data:** none created.
