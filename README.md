# Yield Analysis V4.5 - Yield by Attribute

Added Yield by Attribute analysis.

Default attribute:
- MEDIA_PART_NUM

Also supports:
- HSA_PART_NUM
- PRE_AMP_VENDOR
- FSA_SUPPLIER_0
- DRIVE_PART_NUM
- RUN_TYPE

Calculation by attribute:
- Group by Attribute + selected Operation + derived WW.
- Total = unique analysis records in the group.
- Pass = fail code is N/A / NA / blank / NONE.
- Yield = Pass / Total * 100.

The existing multi-operation selection, WW from DRIVE_SBR_NUM, operation yield, fail details, and cumulative yield remain available.
