# FSK_TEMP_EXT_PARTY_KEYS

---

Replication scratch table used to improve replication performance.

[Back to index](./index.md)

| Column Name               | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ALERT_ID**              | Uniquely identifies an alert.                                                          | NUMBER(12)         | Not Null             | Yes  | No   |
| **EXT_PARTY_ACCOUNT_KEY** | Uniquely identifies an account.                                                        | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**            | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **RUN_DATE**              | System run date.                                                                       | DATE               | Null                 | No   | No   |

[Back to index](./index.md)