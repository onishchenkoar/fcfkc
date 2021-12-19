# FSK_SCENARIO_MESSAGE_DECOMP

---

recompose alert message string

[Back to index](./index.md)

| Column Name                      | Column Definition                           | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------------|:--------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **SCENARIO_MESSAGE_NAME**        | Scenario message name                       | VARCHAR2(35)       | Not Null             | Yes  | No   |
| **MESSAGE_SEGMENT_SEQUENCE_NBR** | Sequence number to identify message segment | NUMBER(10)         | Not Null             | Yes  | No   |
| **MESSAGE_SEGMENT_TEXT**         | Message text fragment                       | VARCHAR2(255)      | Null                 | No   | No   |

[Back to index](./index.md)