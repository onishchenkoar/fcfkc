# FSK_LIST

---

Describes a list. Each row maps to a column in fsc_classifier_fact.

[Back to index](./index.md)

| Column Name              | Column Definition                                                                                                                                                                                                                                        | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **LIST_ID**              | System generated synthetic/surrogate key that uniquely identifies a risk list.                                                                                                                                                                           | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**           | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                                                                                                   | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **LIST_CATEGORY_ID**     | System generated synthetic/surrogate key that uniquely identifies a risk list category.                                                                                                                                                                  | NUMBER(12)         | Null                 | No   | Yes  |
| **LIST_NAME**            | good guy, bad guy, PEP,PSP) -                                                                                                                                                                                                                            | VARCHAR2(35)       | Null                 | No   | No   |
| **LIST_DESC**            | Describes the list that is used to categorize accounts and parties.                                                                                                                                                                                      | VARCHAR2(255)      | Null                 | No   | No   |
| **VALIDATION_TYPE_CODE** | Used for list element validation only. ACC \| PTY \| NONE &mdash; use [fsk_lov](./fsk_lov.md) to match these to a specific table fsc_account_dim \| fsc_party_dim \| NONE. Other values may be added for new list types, but cooresponding entries must also be added to [fsk_lov](./fsk_lov.md). | VARCHAR2(4)        | Not Null             | No   | No   |
| **CREATE_DATE**          | The date the list was created.                                                                                                                                                                                                                           | DATE               | Null                 | No   | No   |
| **CREATE_USER_ID**       | The user who created the list.                                                                                                                                                                                                                           | VARCHAR2(60)       | Null                 | No   | No   |
| **DELETE_DATE**          | The list deletion date.                                                                                                                                                                                                                                  | DATE               | Null                 | No   | No   |
| **DELETE_USER_ID**       | The user who deleted the list.                                                                                                                                                                                                                           | VARCHAR2(60)       | Null                 | No   | No   |
| **LOGICAL_DELETE_IND**   | Has this row been logically deleted Y/N                                                                                                                                                                                                                  | CHAR(1)            | Null                 | No   | No   |

[Back to index](./index.md)
