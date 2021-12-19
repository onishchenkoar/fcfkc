# FSK_ALERT_RISK_FACTOR

---

Attribute Name :   entity_number

[Back to index](./index.md)

| Column Name            | Column Definition                                                                                                                                                                                         | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ENTITY_NUMBER**      | Source system identifier of the entity (Acct, Party, Hhld, Assoc).                                                                                                                                        | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **ALERT_ID**           | System generated synthetic/surrogate key that uniquely identifies an alert.                                                                                                                               | NUMBER(12)         | Not Null             | No   | Yes  |
| **SCENARIO_ID**        | Synthetic unique identifier of Scenarios.                                                                                                                                                                 | NUMBER(12)         | Not Null             | No   | Yes  |
| **SEGMENT_ID**         | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                                                    | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **ENTITY_LEVEL_CODE**  | What type of entity: ACC,PTY,HHD,ASC                                                                                                                                                                      | CHAR(3)            | Not Null             | No   | No   |
| **ACTUAL_VALUES_TEXT** | The actual values that triggered the alert.  For example, a threshold may have been set at $10,000 and a transaction of $14,000 triggered this alert.  The $14,000 figure is captured here for reference. | VARCHAR2(255)      | Null                 | No   | No   |

[Back to index](./index.md)