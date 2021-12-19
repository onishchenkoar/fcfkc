# FSK_CDD_SCORING_EVENT

---

Attribute Name :   cdd_scoring_event_key

[Back to index](./index.md)

| Column Name                      | Column Definition                                                                                                                                                     | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **CDD_SCORING_EVENT_KEY**        | The surrogate key for the CRR_SCORING_EVENT table.                                                                                                                    | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**                   | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **PRIMARY_ENTITY_KEY**           | The key of the entity for the scoring event.                                                                                                                          | NUMBER(12)         | Not Null             | No   | No   |
| **PRIMARY_ENTITY_NUMBER**        | Entity number. If PRIMARY_ENTITY_LEVEL_CODE='PTY', primary_entity_number should be FSC_PARTY_DIM.PARTY_NUMBER.                                                        | VARCHAR2(50)       | Not Null             | No   | No   |
| **PRIMARY_ENTITY_LEVEL_CODE**    | The type of primary entity, for example: household or party.                                                                                                          | CHAR(3)            | Not Null             | No   | No   |
| **CDD_RULE_ID**                  | System generated synthetic/surrogate key that uniquely identifies a row in the  FSK_CDD_SCORING_EVENT table.                                                          | VARCHAR2(32)       | Not Null             | No   | Yes  |
| **VERSION_NO**                   | rule version that generated the score                                                                                                                                 | NUMBER(10)         | Null                 | No   | Yes  |
| **RULE_SCORE**                   | The score for the event, for example: 1, 30, 100.                                                                                                                     | NUMBER(10)         | Null                 | No   | No   |
| **SCORE_CLASSIFICATION_CODE**    | The score classification, for example: low, medium, high.                                                                                                             | VARCHAR2(32)       | Null                 | No   | No   |
| **EVENT_DATE**                   | The date of the scoring event.                                                                                                                                        | DATE               | Not Null             | No   | No   |
| **AUTO_HIGH_IND**                | Indicator flag for marking this scoring event as auto high.                                                                                                           | CHAR(1)            | Null                 | No   | No   |
| **INVESTIGATION_IND**            | Used by IEM to determine which scoring events are to be pushed to ECM.                                                                                                | CHAR(1)            | Null                 | No   | No   |
| **INVESTIGATION_ACTION_CODE**    | Determines what type of entity this will be surfaced as in ECM, for example: 'Indicent' or 'Case'                                                                     | VARCHAR2(32)       | Null                 | No   | No   |
| **CATEGORY_CODE**                | CDD category code.                                                                                                                                                    | VARCHAR2(32)       | Null                 | No   | No   |
| **SCORE_TYPE_CODE**              | CDD score types at different levels. For example ATTR for attribute score, CATEGORY for category score, CATAGGR for category aggregated score, FINAL for final score. | VARCHAR2(32)       | Null                 | No   | No   |
| **INVESTIGATION_TYPE_CD**        | A code corresponding to the investigation type.                                                                                                                       | VARCHAR2(32)       | Null                 | No   | No   |
| **INVESTIGATION_CATEGORY_CD**    | A code corresponding to the investigation category.                                                                                                                   | VARCHAR2(32)       | Null                 | No   | No   |
| **INVESTIGATION_SUBCATEGORY_CD** | A code corresponding to the investigation subcategory.                                                                                                                | VARCHAR2(32)       | Null                 | No   | No   |
| **INVESTIGATION_RK**             | The surrogate key of the investigation object in ECM. The object can be incident, or case, depending on the content of investigation_action_code.                     | NUMBER(12)         | Null                 | No   | No   |
| **INVESTIGATION_STATUS_CD**      | The status code of the investigation object.                                                                                                                          | VARCHAR2(10)       | Null                 | No   | No   |
| **INVESTIGATION_OBJECT_CODE**    | The ECM object type of the CDD investigation . 'C' for Case, 'I' for incident, and 'P' for party.                                                                     | CHAR(1)            | Null                 | No   | No   |

[Back to index](./index.md)
