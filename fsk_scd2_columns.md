# FSK_SCD2_COLUMNS

---

Configurable slowly changing dimension values.

[Back to index](./index.md)

| Column Name        | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **SCD2_KEY**       | Surrogate identifier.                                                                  | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**     | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **TABLE_NAME**     | The name of the table.                                                                 | VARCHAR2(35)       | Not Null             | No   | No   |
| **COLUMN_NAME**    | The name of the column.                                                                | VARCHAR2(35)       | Not Null             | No   | No   |
| **XREF_VALID_IND** | Indicates whether the cross reference is valid.                                        | CHAR(1)            | Not Null             | No   | No   |
| **CREATE_DATE**    | The creation date.                                                                     | DATE               | Not Null             | No   | No   |
| **END_DATE**       | The end date.                                                                          | DATE               | Not Null             | No   | No   |
| **CREATE_USER_ID** | The user who created the SCD2 column.                                                  | VARCHAR(60)        | Not Null             | No   | No   |
| **VERSION_NUMBER** | The version number.                                                                    | NUMBER(10)         | Not Null             | No   | No   |
| **CURRENT_IND**    | Indicates if the row is current. Y/N.                                                  | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)