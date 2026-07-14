# Yield Analysis V4.4

Updates:
- Operation selection uses checkboxes and supports multiple operations.
- Quick buttons: normal operations only, starred operations only, all, and none.
- Default selection includes only operations that do not start with `*`.
- Cumulative yield is calculated in selected production-flow order from top to bottom.
- For each WW: `CUM Yield = Operation 1 Yield × Operation 2 Yield × ... × Operation n Yield`.
- The matrix shows QTY, Operation Yield %, and Cumulative Yield % for each selected operation.
- Fail-code details are displayed for all selected operations.
- WW is still derived from `DRIVE_SBR_NUM` / `DEF_DRIVE_SBR_NUM`, for example `SM50XYDC -> WW50`.
