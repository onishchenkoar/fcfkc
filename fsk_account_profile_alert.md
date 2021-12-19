# FSK_ACCOUNT_PROFILE_ALERT

---

Attribute Name :   alert_id

[Back to index](./index.md)

| Column Name                      | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ALERT_ID**                     | System generated synthetic/surrogate key that uniquely identifies an alert.            | NUMBER(12)         | Not Null             | Yes  | No   |
| **MONTH_KEY**                    | System generated surrogate identifier.                                                 | NUMBER(6,0)        | Not Null             | Yes  | No   |
| **ACCOUNT_NUMBER**               | Natural key of the account.                                                            | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**                   | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **TRANSACTIONS_COUNT**           | Total number of transactions in the account during the profile period.                 | NUMBER(10,0)       | Null                 | No   | No   |
| **DEPOSITS_COUNT**               | Total number of deposits in the account during the profile period.                     | NUMBER(10,0)       | Null                 | No   | No   |
| **WITHDRAWALS_COUNT**            | Total number of withdrawals in the account during the profile period.                  | NUMBER(10,0)       | Null                 | No   | No   |
| **WIRES_COUNT**                  | Total number of wires (in and out) in the account during the profile period.           | NUMBER(10,0)       | Null                 | No   | No   |
| **CASH_TRANSACTIONS_COUNT**      | Total number of cash transactions in the account during the profile period.            | NUMBER(10,0)       | Null                 | No   | No   |
| **ACCOUNT_VALUE_AMOUNT**         | Total Account Market Value at end of period.                                           | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_TRANSACTIONS_AMOUNT**    | Total money amount of all transactions (add up all debits and credits)                 | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_CREDITS_AMOUNT**         | Total credits ($) to the account duing the period.                                     | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_DEBITS_AMOUNT**          | Total debits ($) to the account during the period.                                     | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_CASH_DEBITS_AMOUNT**     | Total Cash debits ($) to the account during the period.                                | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_CASH_CREDITS_AMOUNT**    | Total Cash credits ($) to the account during the period.                               | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_WIRE_CREDITS_AMOUNT**    | Total Wire Credits ($) to the account during the period.                               | NUMBER(18,5)       | Null                 | No   | No   |
| **TOTAL_WIRE_DEBITS_AMOUNT**     | Total Wire debits ($) to the account during the period.                                | NUMBER(18,5)       | Null                 | No   | No   |
| **BEGINNING_BALANCE_AMOUNT**     | Balance at the beginning of the period                                                 | NUMBER(18,5)       | Null                 | No   | No   |
| **AVERAGE_DAILY_BALANCE_AMOUNT** | Average Daily balance during the period                                                | NUMBER(18,5)       | Null                 | No   | No   |
| **ENDING_CASH_BALANCE_AMOUNT**   | Balance at the end of the period.                                                      | NUMBER(18,5)       | Null                 | No   | No   |
| **MAX_ACCOUNT_VALUE_AMOUNT**     | Maximum value of account during the month.                                             | NUMBER(18,5)       | Null                 | No   | No   |
| **MIN_ACCOUNT_VALUE_AMOUNT**     | Minimum value of account during the month.                                             | NUMBER(18,5)       | Null                 | No   | No   |
| **AVG_ACCOUNT_VALUE_AMOUNT**     | Average value of account during the month.                                             | NUMBER(18,5)       | Null                 | No   | No   |
| **CUST_INITIATED_TRANS_COUNT**   | Number of transactions initiated by the customer (vs. by the bank) during the month.   | NUMBER(10)         | Null                 | No   | No   |
| **LARGEST_CREDIT_AMOUNT**        | Largest single credit transaction for the month.                                       | NUMBER(18,5)       | Null                 | No   | No   |
| **LARGEST_DEBIT_AMOUNT**         | Largest single debit transaction for the month.                                        | NUMBER(18,5)       | Null                 | No   | No   |

[Back to index](./index.md)