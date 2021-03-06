# FSK_SCENARIO_MESSAGE

---

This table contains the translated text for Teradata stored procedure messages. The stored procedures use the text to ensure that scenario message output is in the correct language. This table is loaded from the scenario_messages_<language>.sas message file when AML is installed.

[Back to index](./index.md)

| Column Name                                                                                                                                                                                          | Column Definition                                                                                                                                                                                    | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **SCENARIO_MESSAGE_NAME** | Name of the scenario message tag loaded from scenario_messages_<language>.csv using this message string. This value is NOT translated.                                                               | CHAR(35)           | Not Null             | Yes  | No   |
| **SEGMENT_ID**            | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                                               | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **SCENARIO_MESSAGE_TEXT** | Message string text in national language chosen for the install. Loaded from scenario_messages_<language>.csv on AML install. This string is used as a template for creating the actual values text. | VARCHAR2(255)      | Not Null             | No   | No   |

[Back to index](./index.md)
