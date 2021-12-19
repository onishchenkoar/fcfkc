# FSK_REPLICATION_DATES

---

Replication scratch table used to improve replication performance.

[Back to index](./index.md)

| Column Name        | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ALERT_ID**       | Uniquely identifies an alert.                                                          | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**     | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **START_DATE**     | Replication start date.                                                                | DATE               | Null                 | No   | No   |
| **START_DATE_KEY** | Replication start date key.                                                            | NUMBER(8)          | Null                 | No   | No   |

[Back to index](./index.md)