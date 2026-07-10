# Yield Analysis Web App V3 - Yield by Operation Matrix

This version adds a Yield by Operation matrix similar to the reference report.

## Main columns used
- PRODUCT
- DRIVE_SERIAL_NUM
- FISCAL_WEEK
- FAIL_CODE
- OPERATION
- FAILED_STATE
- FAILED_TEST
- EVENT_STATUS
- EVENT_DATE
- RUN_TYPE or BUILD_GROUP for Prime/Rework split

## Logic
- Pass = EVENT_STATUS = P
- Fail = EVENT_STATUS = F
- Yield % = Pass / (Pass + Fail) * 100
- Matrix rows:
  - CUM row = cumulative yield
  - Operation P row = pass/yield summary per operation
  - Fail detail rows = fail-code + failed-state/failed-test grouped under each operation
- Fiscal week columns are generated dynamically from the uploaded CSV.

## Deploy
Replace the root `index.html` in GitHub repo with this file and Commit changes. GitHub Pages will update automatically.
