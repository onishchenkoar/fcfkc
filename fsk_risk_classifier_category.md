# FSK_RISK_CLASSIFIER_CATEGORY

---

Allows user to create groups of related categories.

[Back to index](./index.md)

| Column Name                       | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **RISK_CLASSIFIER_CATEGORY_ID**   | The risk classifier category identifier.                                               | NUMBER(12,0)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**                    | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **RISK_CLASSIFIER_CATEGORY_NAME** | The risk classifier category name.                                                     | VARCHAR2(35)       | Null                 | No   | No   |
| **RISK_CLASSIFIER_CATEGORY_DESC** | The description of the risk classifier category.                                       | VARCHAR2(255)      | Null                 | No   | No   |
| **CREATE_DATE**                   | The date that the risk classifier category was created.                                | DATE               | Null                 | No   | No   |
| **CREATE_USER_ID**                | The user who created the risk classifier category.                                     | VARCHAR2(60)       | Null                 | No   | No   |
| **DELETE_DATE**                   | The date that the risk classifier category was deleted.                                | DATE               | Null                 | No   | No   |
| **DELETE_USER_ID**                | The user who deleted the risk classifier category.                                     | VARCHAR2(60)       | Null                 | No   | No   |
| **LOGICAL_DELETE_IND**            | Has this row been logically deleted Y/N                                                | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)