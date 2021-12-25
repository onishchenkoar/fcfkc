# FSK_CDD_TRIGGERING_VALUES

---

CRR triggering value information.

[Back to index](./index.md)

| Column Name                    | Column Definition                                                                                                                                     | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **CDD_TRIGGERING_VALUE_KEY**   | Unique key for each record.                                                                                                                           | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**                 | Multibank configurations use this column to indicate which bank the record belongs to.                                                                | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **CDD_SCORING_EVENT_KEY**      | The foreign key for the [FSK_CDD_SCORING_EVENT](./fsk_cdd_scoring_event.md) table.                                                                                                    | NUMBER(12)         | Not Null             | No   | Yes  |
| **TRIGGERING_VALUE_ID**        | Unique identifier of each triggering value within a FSK_CDD_TRIGGERING_VALUES.                                                                            | NUMBER(12)         | Null                 | No   | No   |
| **TRIGGERING_CHAR_VALUE**      | Triggering value for **TRIGGERING_VALUE_TYPE_CODE**='CHAR'.                                                                                               | VARCHAR2(35)       | Null                 | No   | No   |
| **TRIGGERING_NUM_VALUE**       | Triggering value for **TRIGGERING_VALUE_TYPE_CODE**='NUM'.                                                                                                | NUMBER(18,5)       | Null                 | No   | No   |
| **TRIGGERING_DATE_VALUE**      | Triggering value for **TRIGGERING_VALUE_TYPE_CODE**='DATE'.                                                                                               | DATE               | Null                 | No   | No   |
| **TRIGGERING_VALUE_TYPE_CODE** | Indicates the triggering value type, for example: number, character, date.                                                                            | VARCHAR2(32)       | Null                 | No   | No   |
| **REF_TABLE_NM**               | The name of the label reference, used for getting the description of triggering value codes. A matching entry should exist in ECM_DB.REF_TABLE_VALUE. | VARCHAR2(30)       | Null                 | No   | No   |

[Back to index](./index.md)
