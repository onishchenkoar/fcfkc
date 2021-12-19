# FSK_ALERT_NEIGHBOR

---

Attribute Name :   alert_id

[Back to index](./index.md)

| Column Name                 | Column Definition                                                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------------|:-----------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ALERT_ID**                | System generated synthetic/surrogate key that uniquely identifies an alert.                                            | NUMBER(12)         | Not Null             | No   | Yes  |
| **TARGET_ACCOUNT_NUMBER**   | The account number related to the alert.                                                                               | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **NEIGHBOR_ACCOUNT_NUMBER** | The number of an account that is considered "close" to the target account.                                             | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**              | Multibank configurations use this column to indicate which bank the record belongs to.                                 | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **DISTANCE**                | A number representing the distance between the target account and the neigbor. Range: 0 (identical) - 0.001 (distant). | NUMBER(4,3)        | Null                 | No   | No   |

[Back to index](./index.md)