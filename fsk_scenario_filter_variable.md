# FSK_SCENARIO_FILTER_VARIABLE

---

The definition of the variables that are calculated by filters.

[Back to index](./index.md)

| Column Name       | Column Definition                                                                                          | Column Data Type   | Column Null Option   | PK   | FK   |
|:------------------|:-----------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **VARIABLE_NAME** | The name of the variable.                                                                                  | VARCHAR2(32)       | Not Null             | Yes  | No   |
| **FILTER_ID**     | Synthetic unique identifier of Filters.                                                                    | NUMBER(12)         | Not Null             | No   | Yes  |
| **SEGMENT_ID**    | Multibank configurations use this column to indicate which bank the record belongs to.                     | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **FUNCTION_NAME** | The name of the function that is used to calculate the value of the variable. For example: average or sum. | VARCHAR2(32)       | Not Null             | No   | No   |
| **VARIABLE_TYPE** | The variable type, for example 'F' for function, or 'V' for value.                                         | CHAR(1)            | Null                 | No   | No   |

[Back to index](./index.md)