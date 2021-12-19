# FSK_TEMP_ASSESS

---

Attribute Name :   party_key

[Back to index](./index.md)

| Column Name     | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **PARTY_KEY**   | Uniquely identifies a party.                                                           | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**  | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **CREATE_DATE** | Assessment create date.                                                                | DATE               | Not Null             | No   | No   |

[Back to index](./index.md)