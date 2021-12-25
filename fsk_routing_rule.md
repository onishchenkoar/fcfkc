# FSK_ROUTING_RULE

---

A set of constraints forming a rule to govern the initial routing of an alert.

[Back to index](./index.md)

| Column Name              | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ROUTING_GROUP_ID**     | Unique identifier.                                                                     | NUMBER(12)         | Not Null             | No   | Yes  |
| **ROUTING_RULE_ID**      | Unique identifier within routing group to identify a rule.                          | NUMBER(12)         | Not Null             | Yes  | No   |
| **ROUTE_ORDER_NUMBER**   | A prioritization of rule execution.  Higher priorities take precedence over lower.     | NUMBER(3)          | Not Null             | Yes  | No   |
| **SEGMENT_ID**           | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **ALERT_TYPE_CD**        | A code corresponding to the alert type.                                                | VARCHAR2(32)       | Null                 | No   | No   |
| **ALERT_CATEGORY_CD**    | A code corresponding to the alert category, for example: DEFAULT, RISKFACT, ATM.       | VARCHAR2(32)       | Null                 | No   | No   |
| **ALERT_SUBCATEGORY_CD** | A code corresponding to the alert subcategory for example: DEFAULT, MANUAL, VELOCITY.  | VARCHAR2(32)       | Null                 | No   | No   |
| **ROUTING_USER_LONG_ID** | USERID of the user who will be the owner of the alert (incident).                      | VARCHAR2(60)       | Null                 | No   | No   |

[Back to index](./index.md)
