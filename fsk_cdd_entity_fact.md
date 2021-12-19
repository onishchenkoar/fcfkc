# FSK_CDD_ENTITY_FACT

---

Attribute Name :   primary_entity_number

[Back to index](./index.md)

| Column Name                       | Column Definition                                                                                                                                                                   | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **PRIMARY_ENTITY_NUMBER**         | Entity number. If PRIMARY_ENTITY_TYPE_CODE='PTY', primary_entity_number should be FSC_PARTY_DIM.PARTY_NUMBER.                                                                       | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **PRIMARY_ENTITY_LEVEL_CODE**     | The type of primary entity, for example: household or party.                                                                                                                        | CHAR(3)            | Not Null             | Yes  | No   |
| **SEGMENT_ID**                    | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                              | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **LAST_CHANGE_DATE**              | The last modified date time.                                                                                                                                                        | DATE               | Not Null             | No   | No   |
| **NEXT_REVIEW_DATE**              | The next scheduled review date. It should be calculated based on some CDD policy.                                                                                                   | DATE               | Null                 | No   | No   |
| **OVERRIDE_SCORE_CLASS_CODE**     | A classification code specified by the investigator when final disposition of the investigation is 'rating change'. A new review date can be re-calculated based on the new rating. | VARCHAR2(32)       | Null                 | No   | No   |
| **FINAL_DISPOSITION_CODE**        | The disposition of the investigation.                                                                                                                                               | VARCHAR2(32)       | Null                 | No   | No   |
| **LAST_REVIEW_DATE**              | The last date that the entity is being reviewed.                                                                                                                                    | DATE               | Null                 | No   | No   |
| **LAST_SCORING_EVENT_KEY**        | The surrogate key of the last scoring event.                                                                                                                                        | NUMBER(12)         | Null                 | No   | No   |
| **LAST_REVIEW_SCORING_EVENT_KEY** | The surrogate key of the scoring event when the entity was last reviewed.                                                                                                           | NUMBER(12)         | Null                 | No   | No   |
| **CURR_REVIEW_SCORING_EVENT_KEY** | The surrogate key of the scoring event when the entity is being reviewed.                                                                                                           | NUMBER(12)         | Null                 | No   | No   |

[Back to index](./index.md)