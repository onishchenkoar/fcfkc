# FSK_CASH_FLOW_BANK_ALERT

---

A record of which banks play a role on a given cash flow transaction.  Roles include REMITTER and BENEFICIARY.

[Back to index](./index.md)

| Column Name         | Column Definition                                                                                                                                                                                                                                            | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ALERT_ID**        | System generated synthetic/surrogate key that uniquely identifies an alert.                                                                                                                                                                                  | NUMBER(12)         | Not Null             | Yes  | No   |
| **BANK_KEY**        | System generated surrogate identifier                                                                                                                                                                                                                        | NUMBER(12)         | Not Null             | Yes  | No   |
| **TRANSACTION_KEY** | Surrogate key.                                                                                                                                                                                                                                               | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**      | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                                                                                                       | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **ROLE**            | Role that the bank plays in the transaction. Starter Values are: BENEFICIARY, REMITTER, CORRESPONDENT, INTERMEDIARY.  Note: Likely not possible to be able to differentiate between correspondent and intermediary - probably best to just use intermediary. | VARCHAR2(20)       | Null                 | No   | No   |
| **SEQUENCE_NUMBER** | Order in which the bank handled the monies.                                                                                                                                                                                                                  | NUMBER(2)          | Null                 | No   | No   |

[Back to index](./index.md)