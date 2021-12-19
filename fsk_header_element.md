# FSK_HEADER_ELEMENT

---

Attribute Name :   header_id

[Back to index](./index.md)

| Column Name              | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **HEADER_ID**            | Name and identifier of the header.                                                     | NUMBER(12)         | Not Null             | No   | Yes  |
| **ELEMENT_NAME**         | Element name.                                                                          | VARCHAR2(35)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**           | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **ELEMENT_TYPE_CODE**    | Datatype: C-Character; N-Numeric                                                       | CHAR(6)            | Not Null             | No   | No   |
| **ELEMENT_LENGTH_COUNT** | Datatype length                                                                        | NUMBER(8)          | Null                 | No   | No   |
| **ELEMENT_FORMAT_CODE**  | Formatting code e.g. $50 or 27.10                                                      | CHAR(12)           | Not Null             | No   | No   |
| **ELEMENT_LABEL_DESC**   | Column name in Core data model.                                                        | VARCHAR2(35)       | Not Null             | No   | No   |
| **ELEMENT_USAGE_DESC**   | How it's used in the code e.g. "Array Element" or "By Variable".                       | VARCHAR2(35)       | Null                 | No   | No   |

[Back to index](./index.md)