# FSK_SCENARIO_FILTER

---

Attribute Name :   filter_id

[Back to index](./index.md)

| Column Name             | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **FILTER_ID**           | Synthetic unique identifier of Filters.                                                | NUMBER(12)         | Not Null             | Yes  | No   |
| **FILTER_ORDER_NUMBER** | The order of the filter in the data step.                                              | NUMBER(5)          | Not Null             | Yes  | No   |
| **SCENARIO_ID**         | Synthetic unique identifier of Scenarios.                                              | NUMBER(12)         | Not Null             | No   | Yes  |
| **SEGMENT_ID**          | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **FILTER_NAME**         | The name of the filter.                                                                | VARCHAR2(35)       | Not Null             | No   | No   |
| **SAVE_TRIG_TRANS_IND** | Indicates whether to save the triggering transaction for this filter.                  | CHAR(1)            | Not Null             | No   | No   |
| **DAYS_NUMBER**         | The number of days to apply the filter.                                                | NUMBER(5)          | Null                 | No   | No   |

[Back to index](./index.md)