# FSK_CDD_RULE

---

Attribute Name :   cdd_rule_id

[Back to index](./index.md)

| Column Name                 | Column Definition                                                                                         | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------------|:----------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **CDD_RULE_ID**             | System generated synthetic/surrogate key that uniquely identifies a row in the  FSK_CDD_RULE table.       | VARCHAR2(32)       | Not Null             | Yes  | No   |
| **VERSION_NO**              | rule version that generated the score                                                                     | NUMBER(10)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**              | Multibank configurations use this column to indicate which bank the record belongs to.                    | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **CURRENT_IND**             | Y if the row is the latest/current version of the rule                                                    | CHAR(1)            | Null                 | No   | No   |
| **CDD_UPDATE_DATE**         | timestamp when  the rule was updated last time                                                            | DATE               | Not Null             | No   | No   |
| **CDD_DEPLOY_DATE**         | timestamp when  the rule was deployed to FCF                                                              | DATE               | Not Null             | No   | No   |
| **CDD_RULE_NAME_ID**        | System generated synthetic/surrogate key that uniquely identifies a row in the  FSK_CDD_RULE table.       | VARCHAR2(32)       | Not Null             | No   | No   |
| **CDD_RULE_NAME**           | rule name                                                                                                 | VARCHAR2(100)      | Not Null             | No   | No   |
| **CDD_RULE_DESCRIPTION_ID** | System generated synthetic/surrogate key that uniquely identifies a row in the  FSK_CDD_RULE table.       | VARCHAR2(32)       | Not Null             | No   | No   |
| **CDD_RULE_DESCRIPTION**    | rule description                                                                                          | VARCHAR2(100)      | Not Null             | No   | No   |
| **CDD_RULE_STATUS_CODE**    | rule status: ACT - active, INA - inactive                                                                 | VARCHAR2(32)       | Not Null             | No   | No   |
| **CDD_RULE_TYPE_CODE**      | The rule type code, for example: attribute rule, aggregation, category aggregation.                       | VARCHAR2(32)       | Not Null             | No   | No   |
| **CDD_RULE_SAVE_ID_FLG**    | 1 if the rule id has to be save in the output data set                                                    | CHAR(1)            | Null                 | No   | No   |
| **CDD_RULE_ORDER_IN_GROUP** | execution order of the rule in the rule group                                                             | NUMBER(12)         | Not Null             | No   | No   |
| **CDD_RULE_GROUP_ID**       | System generated synthetic/surrogate key that uniquely identifies a row in the  FSK_CDD_RULE_GROUP table. | VARCHAR2(32)       | Null                 | No   | Yes  |

[Back to index](./index.md)