# FSK_ACCOUNT_EVENT_ALERT

---

Attribute Name :   alert_id

[Back to index](./index.md)

| Column Name                | Column Definition                                                                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------|:---------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ALERT_ID**               | System generated synthetic/surrogate key that uniquely identifies an alert.                                                            | NUMBER(12)         | Not Null             | Yes  | No   |
| **TRANSACTION_KEY**        | Foreign Key to the transaction dimension.                                                                                              | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**             | Multibank configurations use this column to indicate which bank the record belongs to.                                                 | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **ACCOUNT_KEY**            | Foreign key to the account table.                                                                                                      | NUMBER(12)         | Not Null             | No   | No   |
| **DATE_KEY**               | Note: this is normally a system-generated surrogate key, but for performance reasons we are using a numeric form of the date: yyyymmdd | NUMBER(8,0)        | Not Null             | No   | No   |
| **TRANSACTION_TYPE_KEY**   | Surrogate key.                                                                                                                         | NUMBER(12)         | Not Null             | No   | No   |
| **TIME_KEY**               | Number of Seconds since Midnight                                                                                                       | NUMBER(6)          | Not Null             | No   | No   |
| **COUNTRY_KEY**            | System generated surrogate key.                                                                                                        | NUMBER(5)          | Not Null             | No   | No   |
| **BRANCH_KEY**             | Surrogate identifier.                                                                                                                  | NUMBER(12)         | Not Null             | No   | No   |
| **TRANSACTION_STATUS_KEY** | Foreign key to the transaction status dimension.                                                                                       | NUMBER(5)          | Not Null             | No   | No   |
| **TRIGGER_IND**            | Is this a triggering transaction i.e. did it contribute to the alert?  Y/N                                                             | CHAR(1)            | Null                 | No   | No   |

[Back to index](./index.md)