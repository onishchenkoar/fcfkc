# FSK_LIST_CATEGORY

---

Attribute Name :   list_category_id

[Back to index](./index.md)

| Column Name            | Column Definition                                                                                                                                     | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **LIST_CATEGORY_ID**   | System generated synthetic/surrogate key that uniquely identifies a risk list category.                                                               | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**         | Multibank configurations use this column to indicate which bank the record belongs to.                                                                | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **LIST_CATEGORY_NAME** | Name for the collection of risk lists. (e.g. geographical locations, products and services, customers and entities, account or customer descriptions) | VARCHAR2(35)       | Not Null             | No   | No   |
| **LIST_CATEGORY_DESC** | Long description of category.                                                                                                                         | VARCHAR2(255)      | Null                 | No   | No   |
| **CREATE_DATE**        | The date that the list category was created.                                                                                                          | DATE               | Null                 | No   | No   |
| **CREATE_USER_ID**     | The user who created the list category.                                                                                                               | VARCHAR2(60)       | Null                 | No   | No   |
| **DELETE_DATE**        | The date the list category was deleted.                                                                                                               | DATE               | Null                 | No   | No   |
| **DELETE_USER_ID**     | The user who deleted the list category.                                                                                                               | VARCHAR2(60)       | Null                 | No   | No   |
| **LOGICAL_DELETE_IND** | Has this row been logically deleted Y/N                                                                                                               | CHAR(1)            | Null                 | No   | No   |

[Back to index](./index.md)