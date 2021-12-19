# FSK_TRANSACTION_ALERT

---

transaction.  Storing this data here helps keep the fact table "skinny" and therefore smaller than they would

[Back to index](./index.md)

| Column Name                      | Column Definition                                                                                                                                                                                                              | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ALERT_ID**                     | System generated synthetic/surrogate key that uniquely identifies an alert.                                                                                                                                                    | NUMBER(12)         | Not Null             | Yes  | No   |
| **TRANSACTION_KEY**              | Surrogate key. transaction.  Storing this data here helps keep the fact table "skinny" and therefore smaller than they would otherwise be.                                                                                     | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**                   | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                                                                         | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **DATE_KEY**                     | Note: this is normally a system-generated surrogate key, but for performance reasons we are using a numeric form of the date: yyyymmdd This column has been added to this table to enable table partitioning.                  | NUMBER(8,0)        | Not Null             | No   | No   |
| **TRANSACTION_REFERENCE_NUMBER** | Source system's transaction identifier e.g. deposit number                                                                                                                                                                     | VARCHAR2(50)       | Not Null             | No   | No   |
| **TRANSACTION_DESCRIPTION**      | Free form text description of trade.                                                                                                                                                                                           | VARCHAR2(255)      | Null                 | No   | No   |
| **SECURITY_NAME**                | Name of the equity, bond, currency etc bought or sold.  Could use ticker if preferred.                                                                                                                                         | VARCHAR2(35)       | Null                 | No   | No   |
| **DEAL_NUMBER**                  | Number identifying a trade plus associated settlements.  e.g. Trade is to buy 1mm Euros; settled with two wires each of $500K.  All three transactions are part of the same deal and therefore will have the same deal number. | VARCHAR2(35)       | Null                 | No   | No   |
| **CHECK_NUMBER**                 | The check number of the transaction.                                                                                                                                                                                           | VARCHAR2(10)       | Null                 | No   | No   |
| **MECHANISM_ID**                 | Contains the identifier corresponding to the mechanism description. For example if the transaction is remote deposit, the mechanism id will contain the terminal number.                                                       | VARCHAR2(40)       | Null                 | No   | No   |

[Back to index](./index.md)