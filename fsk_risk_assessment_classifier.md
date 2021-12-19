# FSK_RISK_ASSESSMENT_CLASSIFIER

---

Bridge table between RISK_CLASSIFIER and RISK_ASSESSMENT.

[Back to index](./index.md)

| Column Name            | Column Definition                                                                           | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:--------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **RISK_ASSESSMENT_ID** | System generated synthetic/surrogate key that uniquely identifies a risk assessment record. | NUMBER(12)         | Not Null             | No   | Yes  |
| **SEGMENT_ID**         | Multibank configurations use this column to indicate which bank the record belongs to.      | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **RISK_CLASSIFIER_ID** | A system generated synthetic key used to uniquely identify an instance of an alert event.   | NUMBER(12)         | Not Null             | No   | Yes  |

[Back to index](./index.md)