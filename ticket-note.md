# Ticket note – #12345 (sample, draft for approval)

**QA – Report export (Test environment, sample date)**
Status: Fix not working for large date ranges

**Tested and passed**
- Activity report loads for the last 7 days
- Export for the last 7 days downloads the CSV
- Double-clicking Export sends only one request

**Failed**
- Export for the last 12 months returns an error (API 500 after about 7 seconds). No file is downloaded.

**Manual testing pending**
- Export as a limited-role user
- Export on the mobile app

Evidence attached.
