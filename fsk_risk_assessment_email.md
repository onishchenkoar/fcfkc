# FSK_RISK_ASSESSMENT_EMAIL

---

Attribute Name :   email_id

[Back to index](./index.md)

| Column Name            | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **EMAIL_ID**           | Unique system generated synthetic key used to uniquely identify an alert email.        | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**         | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **RISK_ASSESSMENT_ID** | System generated synthetic/surrogate key that uniquely identifies an alert.            | NUMBER(12)         | Not Null             | No   | Yes  |
| **EMAIL_TO_TEXT**      | Who the email was sent to.                                                             | VARCHAR2(2000)     | Not Null             | No   | No   |
| **EMAIL_CC_TEXT**      | Who was cc'd on the e-mail.                                                            | VARCHAR2(2000)     | Null                 | No   | No   |
| **EMAIL_SUBJECT_DESC** | e-mail subject                                                                         | VARCHAR2(255)      | Null                 | No   | No   |
| **EMAIL_MESSAGE_TEXT** | e-mail body                                                                            | VARCHAR2(4000)     | Null                 | No   | No   |
| **CREATE_DATE**        | Date the e-mail was added to the alert.                                                | DATE               | Not Null             | No   | No   |
| **CREATE_USER_ID**     | Which user added the e-mail to the alert.                                              | VARCHAR2(60)       | Not Null             | No   | No   |

[Back to index](./index.md)