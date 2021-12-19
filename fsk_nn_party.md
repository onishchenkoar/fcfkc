# FSK_NN_PARTY

---

Stores data related to near neighbor party functionality.

[Back to index](./index.md)

| Column Name      | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ALERT_ID**     | System generated synthetic/surrogate key that uniquely identifies an alert.            | NUMBER(12)         | Not Null             | Yes  | No   |
| **PARTY_NUMBER** | Party Number                                                                           | VARCHAR2(76)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**   | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |

[Back to index](./index.md)