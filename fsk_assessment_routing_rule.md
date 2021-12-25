# FSK_ASSESSMENT_ROUTING_RULE

---

A set of constraints forming a rule to govern the initial routing of an alert.

[Back to index](./index.md)

| Column Name                     | Column Definition                                                                            | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------------------|:---------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ROUTING_RULE_ID**             | Unique identifier within **ROUTING_GROUP_ID** to identify a routing rule.                        | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**                  | Multibank configurations use this column to indicate which bank the record belongs to.       | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **LIST_ID**                     | System generated synthetic/surrogate key that uniquely identifies a risk list.               | NUMBER(12)         | Null                 | No   | Yes  |
| **RISK_ASSESSMENT_COLUMN_NAME** | Column in the fsk_risk_assessment table which contains the value that this rule is based on. | VARCHAR2(30)       | Not Null             | No   | No   |
| **ROUTE_PRIORITY_NUMBER**       | A prioritization of rule execution.  Higher priorities take precedence over lower.           | NUMBER(3)          | Null                 | No   | No   |
| **ASSESSMENT_TYPE_CD**          | A code corresponding to the assessment routing rule type.                                    | VARCHAR2(32)       | Null                 | No   | No   |
| **ASSESSMENT_CATEGORY_CD**      | A code corresponding to the assessment routing rule category.                                | VARCHAR2(32)       | Null                 | No   | No   |
| **ASSESSMENT_SUBCATEGORY_CD**   | A code corresponding to the assessment routing rule subcategory.                             | VARCHAR2(32)       | Null                 | No   | No   |
| **ROUTING_USER_LONG_ID**        | USERID of the user who will be the owner of the assessment routing rule.                     | VARCHAR2(60)       | Null                 | No   | No   |

[Back to index](./index.md)
