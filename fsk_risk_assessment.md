# FSK_RISK_ASSESSMENT

---

Details of a potentially suspicious entity identified as a result of scenarios and risk factors triggering.

[Back to index](./index.md)

| Column Name                      | Column Definition                                                                                               | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------------|:----------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **RISK_ASSESSMENT_ID**           | System generated synthetic/surrogate key that uniquely identifies a risk assessment record.                     | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**                   | Multibank configurations use this column to indicate which bank the record belongs to.                          | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **RISK_ASSESSMENT_STATUS_CODE**  | Status: Active (ACT), Closed (CLS), Checked Out (OUT)                                                            | CHAR(3)            | Not Null             | No   | No   |
| **RISK_CLASSIFICATION**          | The risk_classification that the party had prior to this assessment.                                            | NUMBER(1)          | Null                 | No   | No   |
| **PROPOSED_RISK_CLASSIFICATION** | The proposed risk classification for the party.                                                                 | NUMBER(1)          | Null                 | No   | No   |
| **PARTY_NUMBER**                 | Natural key of primary entity (party, account, hhld) associated with the risk assessment record.                | VARCHAR2(50)       | Not Null             | No   | No   |
| **PARTY_KEY**                    | Surrogate key of primary entity (party, account, hhld) associated with the risk assessment record               | NUMBER(12)         | Null                 | No   | No   |
| **PARTY_NAME**                   | The party name for the risk assessment.                                                                         | VARCHAR2(35)       | Null                 | No   | No   |
| **STARTING_MONTH_KEY**           | Which batch asof date the assessment was generated from.                                                        | NUMBER(6,0)        | Null                 | No   | No   |
| **RISK_ASSESSMENT_DURATION**     | Number of months of risk_classifier_fact data that were considered in producing this risk_classification value. | NUMBER(3)          | Not Null             | No   | No   |
| **CREATE_DATE**                  | When the RA record was created                                                                                  | DATE               | Not Null             | No   | No   |
| **CREATE_USER_ID**               | User who inserted the record into the database.                                                                 | VARCHAR2(60)       | Not Null             | No   | No   |
| **EMPLOYEE_IND**                 | Is the entity of interest an employee of the client? Y/N                                                        | CHAR(1)            | Null                 | No   | No   |
| **VERSION_NUMBER**               | Used to implement optimistic locking.                                                                           | NUMBER(10)         | Not Null             | No   | No   |
| **LOGICAL_DELETE_IND**           | Has the record been logically deleted? Y/N                                                                      | CHAR(1)            | Not Null             | No   | No   |
| **ASSESSMENT_TYPE_CD**           | The assessment type code.                                                                                       | VARCHAR2(32)       | Null                 | No   | No   |
| **ASSESSMENT_CATEGORY_CD**       | The assessment category code.                                                                                   | VARCHAR2(32)       | Null                 | No   | No   |
| **ASSESSMENT_SUBCATEGORY_CD**    | The assessment subcategory code.                                                                                | VARCHAR2(32)       | Null                 | No   | No   |
| **OWNER_USER_LONG_ID**           | USERID of the user who will be the owner of the alert (incident).                                               | VARCHAR2(60)       | Null                 | No   | No   |

[Back to index](./index.md)
