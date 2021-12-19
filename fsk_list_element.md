# FSK_LIST_ELEMENT

---

Attribute Name :   list_element_id

[Back to index](./index.md)

| Column Name            | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **LIST_ELEMENT_ID**    | System generated synthetic/surrogate key that uniquely identifies an risk list element | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**         | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **LIST_ID**            | System generated synthetic/surrogate key that uniquely identifies a risk list.         | NUMBER(12)         | Null                 | No   | Yes  |
| **LIST_ELEMENT_DESC**  | The description of the list element.                                                   | VARCHAR2(35)       | Null                 | No   | No   |
| **LIST_ELEMENT_VALUE** | A value that is used to categorize accounts and parties.                               | VARCHAR2(75)       | Not Null             | No   | No   |
| **CREATE_DATE**        | The date that the list element was created.                                            | DATE               | Null                 | No   | No   |
| **CREATE_USER_ID**     | The user who created the list element.                                                 | VARCHAR2(60)       | Null                 | No   | No   |
| **DELETE_DATE**        | The date that the list element was deleted.                                            | DATE               | Null                 | No   | No   |
| **DELETE_USER_ID**     | The user who deleted the list element.                                                 | VARCHAR2(60)       | Null                 | No   | No   |
| **LOGICAL_DELETE_IND** | Has this row been logically deleted Y/N                                                | CHAR(1)            | Null                 | No   | No   |

[Back to index](./index.md)