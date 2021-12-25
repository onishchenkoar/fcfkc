# FSK_SCENARIO_ALERT_COLUMN

---

Stores additional columns for a scenario or risk factor when an alert is output.

[Back to index](./index.md)

| Column Name           | Column Definition                                                                                                                                                                                                                  | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **SCENARIO_ID**       | Synthetic unique identifier of Scenarios.                                                                                                                                                                                          | NUMBER(12)         | Not Null             | No   | Yes  |
| **COLUMN_NAME**       | The name of the additional column that is saved when an alert is output.                                                                                                                                                           | CHAR(32)           | Not Null             | Yes  | No   |
| **SEGMENT_ID**        | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                                                                             | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **COLUMN_USAGE_CODE** | The column usage code. For example, U:  UI - only used for UI purposes (display available HP C variables for example). S:  Storage - only used for storage (for example into [FSK_ENHANCED_ALERT](./fsk_enhanced_alert.md)) . B:  Both - Both UI and Storage. | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)
