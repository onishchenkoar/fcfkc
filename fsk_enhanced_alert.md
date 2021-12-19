# FSK_ENHANCED_ALERT

---

Attribute Name :   alert_id

[Back to index](./index.md)

| Column Name                | Column Definition                                                                                                                    | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------|:-------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ALERT_ID**               | System generated synthetic/surrogate key that uniquely identifies an alert.                                                          | NUMBER(12)         | Not Null             | No   | Yes  |
| **COLUMN_NAME**            | The name of the additional column that is saved when an alert is output.                                                             | CHAR(32)           | Not Null             | Yes  | No   |
| **SEGMENT_ID**             | Multibank configurations use this column to indicate which bank the record belongs to.                                               | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **COLUMN_TYPE_CODE**       | The column type. For example, N for numeric, C for character.                                                                        | CHAR(1)            | Not Null             | No   | No   |
| **COLUMN_VALUE_NUMBER**    | If the column type is numeric, this is the numeric value of the column. If the column type is not numeric, this value is NULL.       | DOUBLE PRECISION   | Null                 | No   | No   |
| **COLUMN_VALUE_CHAR_TEXT** | If the column type is character, this is the character value of the column. If the column type is not character, this value is NULL. | VARCHAR2(4000)     | Null                 | No   | No   |

[Back to index](./index.md)