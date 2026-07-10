# Yield Analysis Web App V3.3 - Correct FAIL_CODE Logic

Important logic update from user requirement:

1. Summary must be by week and by operation.
2. PASSER for each operation is determined by `FAIL_CODE = N/A`.
3. Operation total is the number of drives entering that operation.
4. Fail percentage is calculated as:
   fail code drive count / total drives entering that operation * 100
5. Operation yield is:
   N/A count / total operation count * 100
   Example: 100 drives enter SCOPY and 1 drive fails FAIL_CODE 11049, SCOPY yield = 99%.
6. Default count mode is Unique Drive per Operation.
7. Operation order: SCOPY, PRE2, CAL2, FNC2, CRT2, FIN2.

Deploy:
Replace root `index.html` in the GitHub repository and commit changes.
