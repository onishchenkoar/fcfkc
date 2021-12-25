# FSK_CDD_RULE_GROUP

---

Definitions for Customer Due Diligence Rule Groups

[Back to index](./index.md)

| Column Name                        | Column Definition                                                                                                                   | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------------------|:------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **CDD_RULE_GROUP_ID**              | System generated synthetic/surrogate key that uniquely identifies a row in the  FSK_CDD_RULE_GROUP table.                           | VARCHAR2(32)       | Not Null             | Yes  | No   |
| **VERSION_NO**                     | Rule group version number                                                                                                           | NUMBER(10)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**                     | Multibank configurations use this column to indicate which bank the record belongs to.                                              | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **CURRENT_IND**                    | Y if the row is the latest/current version of the rule group                                                                        | CHAR(1)            | Null                 | No   | No   |
| **CDD_UPDATE_DATE**                | Timestamp when  the rule group was updated last time                                                                                | DATE               | Not Null             | No   | No   |
| **CDD_DEPLOY_DATE**                | Timestamp when  the rule group was deployed to FCF                                                                                  | DATE               | Not Null             | No   | No   |
| **CDD_RULE_GROUP_FILE_NAME**       | File name of the generated SAS code for the rule group                                                                              | VARCHAR2(128)      | Not Null             | No   | No   |
| **CDD_RULE_GROUP_CATEGORY_CODE**   | Rule group category: COUNTRY, PRODUCT, ENTIRY, TRANS, etc.                                                                          | VARCHAR2(32)       | Not Null             | No   | No   |
| **CDD_RULE_GROUP_DESC_ID**         | System generated synthetic/surrogate key that uniquely identifies a row in the  FSK_CDD_RULE_GROUP table.                           | VARCHAR2(32)       | Not Null             | No   | No   |
| **CDD_RULE_GROUP_DESCRIPTION**     | Rule group description                                                                                                              | VARCHAR2(100)      | Not Null             | No   | No   |
| **CDD_RULE_GROUP_NAME_ID**         | System generated synthetic/surrogate key that uniquely identifies a row in the  FSK_CDD_RULE_GROUP table.                           | VARCHAR2(32)       | Not Null             | No   | No   |
| **CDD_RULE_GROUP_NAME**            | Rule group name                                                                                                                     | VARCHAR2(100)      | Not Null             | No   | No   |
| **CDD_RULE_GROUP_INPUT_DS_NAME**   | Input data set name for the rule group execution, used only for Attribute and Category rule groups, NULL for aggregated rule groups | VARCHAR2(32)       | Null                 | No   | No   |
| **CDD_RULE_GROUP_BY_VAR_1_NAME**   | First BY variable to process the input data set                                                                                     | VARCHAR2(32)       | Null                 | No   | No   |
| **CDD_RULE_GROUP_BY_VAR_2_NAME**   | Second BY variable to process the input data set                                                                                    | VARCHAR2(32)       | Null                 | No   | No   |
| **CDD_RULE_GROUP_LEVEL**           | Execution order of the rule group in the CRR process (several groups per dataset are supported)                                     | NUMBER(10)         | Null                 | No   | No   |
| **CDD_RULE_GROUP_ORDER_IN_LEVEL**  | Execution order of the rule group order within the same level                                                                       | NUMBER(10)         | Null                 | No   | No   |
| **CDD_RULE_GROUP_SAVE_TO_KC_FLG**  | Save the datastep scores to FCF KC                                                                                                  | CHAR(1)            | Null                 | No   | No   |
| **CDD_RULE_GROUP_SAVE_TRIG_V_FLG** | Save the score triggering values to FCF KC                                                                                          | CHAR(1)            | Null                 | No   | No   |

[Back to index](./index.md)
