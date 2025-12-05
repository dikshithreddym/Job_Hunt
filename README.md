# Job Hunt

Automated daily ML/AI job scraper for Canada. Scrapes job boards, filters out senior/irrelevant roles, writes results to Google Sheets (Master + Today tabs), auto-fits columns, sets row height, and emails a completion notice.

## Setup
- Add required GitHub Actions secrets: `GSHEETS_CREDS_JSON`, `SHEET_URL`, `GMAIL_USER`, `MAIL_APP_PASSWORD`, `TO_EMAIL`.
- Service account must have Editor access to the spreadsheet.

## Local Run
```pwsh
pip install -r requirements.txt
python job_scraper.py
```

## CI Run
Configured in `.github/workflows/scrape.yml` to run daily at ~08:00 AM Toronto.
