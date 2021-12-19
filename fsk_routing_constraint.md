# FSK_ROUTING_CONSTRAINT

---

A specific constraint within a rule used to determine initial routing of an alert.  e.g. money_laundering_risk_score >

[Back to index](./index.md)

| Column Name                 | Column Definition                                                                                          | Column Data Type   | Column Null Option   | PK   | FK      |
|:----------------------------|:-----------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:--------|
| **ROUTING_GROUP_ID**        | Unique identifier.                                                                                         | NUMBER(12)         | Not Null 700.        | No   | Yes     |
| **ROUTING_RULE_ID**         | Unique identifier within routing_group_id to identify a rule.                                              | NUMBER(12)         | Not Null             | No   | Yes     |
| **CONSTRAINT_ORDER_NUMBER** | Unique sequence number within routing_group_id and routing_rule_id used to identify a specific constraint. | NUMBER(2)          | Not Null             | Yes  | No      |
| **SEGMENT_ID**              | Multibank configurations use this column to indicate which bank the record belongs to.                     | VARCHAR2(128)      | Not Null             | No   | Yes     |
| **COLUMN_NAME**             | Name of a column in FSK_ALERT on which to constrain.                                                       | VARCHAR2(35)       | Null                 | No   | No      |
| **OPERATOR_DESC**           | The logical operator forming the constraint. e.g. > or <.                                                  | CHAR(6)            | Null                 | No   | No 700. |
| **VALUE_DESC**              | The value to compare the column against.                                                                   | VARCHAR2(1024)     | Null                 | No   | No      |
| **COMPOUND_OPERATOR_NAME**  | The operator used to combine constraints within a rule.                                                    | CHAR(4)            | Null                 | No   | No      |

[Back to index](./index.md)