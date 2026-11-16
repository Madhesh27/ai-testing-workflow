# Test plan – Ticket #<ID> – <short title>

**Goal:** <what the fix should do>
**Environment:** <TEST environment>  ·  **Account:** <test account>

Tag every scenario:
- `[AI]` – the agent may run it
- `[Manual: reason]` – a person must run it (the agent only lists it)
- `[read-only]` or `[creates/deletes test data]`
- `[needs 2nd user]` when a second login is required

---

1. [AI] [read-only] <Scenario name>
   Steps: <step> → <step> → <step>
   Expected: <expected result>

2. [AI] [creates/deletes test data] <Scenario name>
   Steps: <step> → <step> → delete the test data afterwards
   Expected: <expected result>

3. [Manual: <reason>] [needs 2nd user] <Scenario name>
   Steps: <step> → <step>
   Expected: <expected result>

**Edge cases to try:** double click · cancel then retry · reload mid-way · duplicates · empty / very large input
