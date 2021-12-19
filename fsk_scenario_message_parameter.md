# FSK_SCENARIO_MESSAGE_PARAMETER

---

The parameters for messages that are saved with alerts.

[Back to index](./index.md)

| Column Name                | Column Definition                                                                           | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------|:--------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **PARAMETER_NUMBER**       | The order of the message parameter.                                                         | NUMBER(5)          | Not Null             | Yes  | No   |
| **SCENARIO_ID**            | Synthetic unique identifier of Scenarios.                                                   | NUMBER(12)         | Not Null             | No   | Yes  |
| **SEGMENT_ID**             | Multibank configurations use this column to indicate which bank the record belongs to.      | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **MESSAGE_PARAMETER**      | The value for the parameter for a message. This can be a variable name or a constant value. | VARCHAR2(32)       | Not Null             | No   | No   |
| **MESSAGE_PARAMETER_TYPE** | The parameter value type.                                                                   | CHAR(1)            | Not Null             | No   | No   |
| **VARIABLE_FORMAT**        | The format of the variable if it is required.                                               | VARCHAR2(32)       | Null                 | No   | No   |

[Back to index](./index.md)