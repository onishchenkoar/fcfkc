# FSK_ALERT_REMINDER

---

Via the UI, users can request to be reminded to review an alert after a certain number of days.  This table stores those requests.  A batch job reviews this table daily and generates reminder e-mails as necessary.

[Back to index](./index.md)

| Column Name           | Column Definition                                                                            | Column Data Type   | Column Null Option                                                                                          | PK   | FK   |
|:----------------------|:---------------------------------------------------------------------------------------------|:-------------------|:------------------------------------------------------------------------------------------------------------|:-----|:-----|
| **ALERT_ID**          | System generated synthetic/surrogate key that uniquely identifies an alert.                  | NUMBER(12)         | Not Null                                                                                                    | No   | Yes  |
| **REMINDER_DATE**     | Date on which the e-mail should be sent (i.e. should first appear in the recipient's inbox). | DATE               | Not Null                                                                                                    | Yes  | No   |
| **SEGMENT_ID**        | Multibank configurations use this column to indicate which bank the record belongs to.       | VARCHAR2(128)      | Not Null                                                                                                    | No   | Yes  |
| **USER_LONG_ID**      | User ID from metadata (In SMC the Name field in the General tab for a user) e.g. kebett      | VARCHAR2(60)       | Not Null | Yes  | No   |
| **REMINDER_SENT_IND** | Has the reminder been sent (Y/N)?                                                            | CHAR(1)            | Null                                                                                                        | No   | No   |

[Back to index](./index.md)
