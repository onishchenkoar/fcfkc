# FSK_SCENARIO_LOCALIZED_MSG

---

Attribute Name :   scenario_id

[Back to index](./index.md)

| Column Name               | Column Definition                                                                                                                                                                                                                                                                       | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **SCENARIO_ID**           | Synthetic unique identifier of Scenarios.                                                                                                                                                                                                                                               | NUMBER(12)         | Not Null             | No   | Yes  |
| **SEGMENT_ID**            | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                                                                                                                                  | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **LOCALE**                | A locale supported by the application. The locale should follow the Java locale naming convention: a valid 2-letter lowercase ISO 639 language code optionally appended with an underscore and a 2-letter uppercase ISO 3166 country code. For example "en", "en_US", "en_GB", "fr_FR". | VARCHAR2(5)        | Not Null             | No   | No   |
| **SCENARIO_MESSAGE_TEXT** | The scenario message text.                                                                                                                                                                                                                                                              | VARCHAR2(255)      | Not Null             | No   | No   |

[Back to index](./index.md)