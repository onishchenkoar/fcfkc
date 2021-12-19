# FSK_CDD_RULE_PARAMETER

---

Definitions for Customer Due Diligence Rule Parameters

[Back to index](./index.md)

| Column Name                   | Column Definition                                                                                   | Column Data Type   | Column Null Option   | PK   | FK   |
|:------------------------------|:----------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **CDD_RULE_VERSION_NO**       | rule version in FSK_CDD_RULE for the parameter                                                      | NUMBER(10)         | Not Null             | Yes  | No   |
| **CDD_RULE_PARM_NAME**        | Parameter name                                                                                      | VARCHAR2(100)      | Not Null             | Yes  | No   |
| **SEGMENT_ID**                | Multibank configurations use this column to indicate which bank the record belongs to.              | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **CDD_RULE_ID**               | System generated synthetic/surrogate key that uniquely identifies a row in the  FSK_CDD_RULE table. | VARCHAR2(32)       | Not Null             | No   | Yes  |
| **CDD_RULE_PARM_DESC_ID**     | Parameter description ID                                                                            | VARCHAR2(32)       | Not Null             | No   | No   |
| **CDD_RULE_PARM_DESCRIPTION** | Parameter description                                                                               | VARCHAR2(100)      | Not Null             | No   | No   |
| **CDD_RULE_PARM_TYPE_CODE**   | Parameter type                                                                                      | VARCHAR2(32)       | Not Null             | No   | No   |
| **CDD_RULE_PARM_VAL**         | Parameter value                                                                                     | VARCHAR2(1024)     | Not Null             | No   | No   |

[Back to index](./index.md)