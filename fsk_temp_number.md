# FSK_TEMP_NUMBER

---

Temporary table used to improve performance.

[Back to index](./index.md)

| Column Name               | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **PRIMARY_ENTITY_NUMBER** | Natural key of entity being processed.                                                 | VARCHAR2(75)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**            | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |

[Back to index](./index.md)