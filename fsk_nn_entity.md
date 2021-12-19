# FSK_NN_ENTITY

---

Stores data related to near neighbor entity  functionality.

[Back to index](./index.md)

| Column Name                   | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:------------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **PRIMARY_ENTITY_NUMBER**     | Natural key of primary entity (party, account, hhld) associated with the alert.        | VARCHAR2(76)       | Not Null             | Yes  | No   |
| **PRIMARY_ENTITY_LEVEL_CODE** | ACC, PTY, HHD, ASC, BLT                                                                | CHAR(3)            | Not Null             | Yes  | No   |
| **ALERT_ID**                  | System generated synthetic/surrogate key that uniquely identifies an alert.            | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**                | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |

[Back to index](./index.md)