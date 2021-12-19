# FSK_SEQUENCE

---

Attribute Name :   segment_id

[Back to index](./index.md)

| Column Name          | Column Definition                                                                                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **SEGMENT_ID**       | Multibank configurations use this column to indicate which bank the record belongs to.                                                                 | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **NEXT_SEQUENCE_ID** | The next identifier available to be used.  The user should read this value and immediately increment, update and commit to allow the next user access. | NUMBER(12)         | Not Null             | No   | No   |

[Back to index](./index.md)