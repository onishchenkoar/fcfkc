# FSK_SCENARIO_PARAMETER

---

Details of parameters used in the scenario.

[Back to index](./index.md)

| Column Name        | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **SCENARIO_ID**    | Synthtic key used to uniquely identify a rule.                                         | NUMBER(12)         | Not Null             | No   | Yes  |
| **PARM_NAME**      | Label used to define a rule parameter e.g. DURATION.                                   | VARCHAR2(32)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**     | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **PARM_VALUE**     | The value used for the given parameter for this rule execution.                        | VARCHAR2(1024)     | Not Null             | No   | No   |
| **PARM_TYPE_DESC** | Parameters can be specified in three forms: Constant, Variable, or List.               | VARCHAR2(32)       | Not Null             | No   | No   |
| **PARM_DESC**      | Freeform description of the parameter.                                                 | VARCHAR2(255)      | Not Null             | No   | No   |

[Back to index](./index.md)