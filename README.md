# Yield Analysis Web App V4.1 - XLSX/CSV + SUMMIT aliases

Updated for the uploaded SUMMIT workbook.

## Added
- Accepts `.csv`, `.xlsx`, `.xls`
- Supports SUMMIT column aliases:
  - Operation: `DEF_OPERATION` or `OPERATION`
  - Fail code: `FAIL_DTL_FAIL_CODE` or `FAIL_CODE`
  - Week: `BRTH_DT_FISCAL_WEEK`, `EVT_DT_FISCAL_WEEK`, `WW`, or `FISCAL_WEEK`
  - Drive serial: `DRIVE_DIM_DRIVE_SERIAL_NUM` or `DRIVE_SERIAL_NUM`
  - Run type: `DEF_RUN_TYPE` or `RUN_TYPE`
  - Event date: `DEF_ETL_LOAD_DATE`, `EVT_DT_ACTUAL_DATE`, `DEF_BIRTH_DATE`, or `EVENT_DATE`

## File size guidance
- CSV: chunk processing, recommended up to 300-500 MB depending on machine.
- XLSX: loaded into browser memory, recommended up to ~50-100 MB. For larger files, save/export as CSV first.

## Logic
- PASSER = fail code is `N/A`, `NA`, blank, or `NONE`
- Failure = any other fail code
- Yield = PASSER count / operation total * 100
- Fail detail % = fail code qty / operation total * 100

Deploy by replacing root `index.html` in GitHub Pages repo.
