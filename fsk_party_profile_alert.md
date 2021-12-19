# FSK_PARTY_PROFILE_ALERT

---

Attribute Name :   alert_id

[Back to index](./index.md)

| Column Name                   | Column Definition                                                                                               | Column Data Type   | Column Null Option   | PK   | FK   |
|:------------------------------|:----------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ALERT_ID**                  | System generated synthetic/surrogate key that uniquely identifies an alert.                                     | NUMBER(12)         | Not Null             | Yes  | No   |
| **MONTH_KEY**                 | Meaningful surrogate key of format yyyymm.                                                                      | NUMBER(6,0)        | Not Null             | Yes  | No   |
| **PARTY_NUMBER**              | Source system's customer identifier..                                                                           | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**                | Multibank configurations use this column to indicate which bank the record belongs to.                          | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **AGGREGATE_ASSETS_AMOUNT**   | Total assets across all accounts.  Only includes assets, does not include loan amounts.                         | NUMBER(18,5)       | Null                 | No   | No   |
| **TRANSACTIONS_COUNT**        | Total number of transactions of accounts associated with this party during the profile period.                  | NUMBER(10,0)       | Null                 | No   | No   |
| **DEPOSITS_COUNT**            | The total number of deposits to accounts associated with this party during the profile period.                  | NUMBER(10,0)       | Null                 | No   | No   |
| **WITHDRAWALS_COUNT**         | Total number of withdrawls from accounts associated with this party during the profile period.                  | NUMBER(10,0)       | Null                 | No   | No   |
| **WIRES_COUNT**               | Total number of wires on accounts associated with this party during the profile period.                         | NUMBER(10,0)       | Null                 | No   | No   |
| **CASH_TRANSACTIONS_COUNT**   | Total number of cash transaction during the profile period.                                                     | NUMBER(10,0)       | Null                 | No   | No   |
| **ACCOUNT_VALUE_AMOUNT**      | Total market value of accounts associated with this party at the end of the profile period.                     | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_TRANSACTIONS_AMOUNT** | Total money amount of all transactions (add up all debits and credits) for accounts associated with this party. | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_CREDITS_AMOUNT**      | Total money amount of all credits for accounts associated with this party.                                      | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_DEBITS_AMOUNT**       | Total money amount of all debits for accounts associated with this party.                                       | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_CASH_DEBITS_AMOUNT**  | Total money amount of all cash debits for accounts associated with this party.                                  | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_CASH_CREDITS_AMOUNT** | Total money amount of all cash credits for accounts associated with this party.                                 | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_WIRE_CREDITS_AMOUNT** | Total Wire Credits ($) to all accounts for the party during the period.                                         | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_WIRE_DEBITS_AMOUNT**  | Total Wire debits ($) to all accounts for the party during the period.                                          | NUMBER(18,5)       | Null                 | No   | No   |
| **LARGEST_CREDIT_AMOUNT**     | Largest credit to any account associated with this party during the profile period.                             | NUMBER(18,5)       | Null                 | No   | No   |
| **LARGEST_DEBIT_AMOUNT**      | Largest debit to any account associated with this party during the profile period.                              | NUMBER(18,5)       | Null                 | No   | No   |
| **FUNDS_PAYMENT_SVCS_COUNT**  | Number of funds payment services to any account associated with this party during the profile period.           | NUMBER(10)         | Null                 | No   | No   |
| **FUNDS_TRANSFER_COUNT**      | Number of transfers to all accounts associated with this party during the profile period.                       | NUMBER(10)         | Null                 | No   | No   |
| **MONETARY_INSTRUMENT_COUNT** | Number of monetary instrument transactions on all accounts.                                                     | NUMBER(10)         | Null                 | No   | No   |

[Back to index](./index.md)