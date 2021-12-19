# FSK_SCENARIO_FILTER_CONSTRAINT

---

Attribute Name :   constraint_order_number

[Back to index](./index.md)

| Column Name                 | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **CONSTRAINT_ORDER_NUMBER** | The order that the constraint within the logical expression.                           | NUMBER(5)          | Not Null             | Yes  | No   |
| **FILTER_ID**               | Synthetic unique identifier of Filters.                                                | NUMBER(12)         | Not Null             | No   | Yes  |
| **SEGMENT_ID**              | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **LEFT_OPERAND**            | The left operand of the constraint.                                                    | VARCHAR2(32)       | Not Null             | No   | No   |
| **LEFT_OPERAND_TYPE**       | The type of the left operand.                                                          | CHAR(1)            | Not Null             | No   | No   |
| **CONSTRAINT_OPERATOR**     | The operator of the constraint, for example '=', 'NOT IN', '>'.                        | VARCHAR2(6)        | Not Null             | No   | No   |
| **RIGHT_OPERAND**           | The right operand of the constraint.                                                   | VARCHAR2(256)      | Not Null             | No   | No   |
| **RIGHT_OPERAND_TYPE**      | The type of the right operand.                                                         | CHAR(1)            | Not Null             | No   | No   |
| **COMPOUND_OPERATOR**       | The compound operator for the constraint, for example: 'or', 'and'.                    | CHAR(3)            | Not Null             | No   | No   |

[Back to index](./index.md)