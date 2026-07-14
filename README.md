# Yield Web App V4.8.5 - EC Detail

Full replacement based on V4.8.4.

New behavior:
- Each selected operation retains its main QTY and Yield row.
- Directly below each operation, EC detail rows show fail-code QTY and EC percentage for every hierarchical group.
- EC % = EC quantity / total drives entering that operation in that group * 100.
- EC codes are ranked by total occurrence for the selected product and limited by the EC-per-operation control.
- EC detail can be shown or hidden.
- Existing decode-before-group, hierarchical sorting, cumulative yield, themes, and CSV export remain intact.
