# FSK_SCENARIO_MESSAGE_DECOMP

---

Used in AlertStringBuild to decompose message, put variable values in place of pound sign parameters, and

[Back to index](./index.md)

| Column Name                      | Column Definition                           | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------------|:--------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **SCENARIO_MESSAGE_NAME**        | Scenario message name                       | VARCHAR2(35)       | Not Null             | Yes  | No   |
| **MESSAGE_SEGMENT_SEQUENCE_NBR** | Sequence number to identify message segment | NUMBER(10)         | Not Null             | Yes  | No   |
| **MESSAGE_SEGMENT_TEXT**         | Message text fragment                       | VARCHAR2(255)      | Null                 | No   | No   |

[Back to index](./index.md)