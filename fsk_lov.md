# FSK_LOV

---

Attribute Name :   lov_type_name

[Back to index](./index.md)

| Column Name                  | Column Definition                                                                                                        | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------------|:-------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **LOV_TYPE_NAME**            | Which list of values. e.g. "Alert Type", "Rule Type".                                                                    | CHAR(18)           | Not Null             | Yes  | No   |
| **LOV_TYPE_CODE**            | The code value e.g. "ACT"                                                                                                | CHAR(3)            | Not Null             | Yes  | No   |
| **SEGMENT_ID**               | Multibank configurations use this column to indicate which bank the record belongs to.                                   | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **LOV_TYPE_DESC**            | A description of the code. e.g. "Active"                                                                                 | VARCHAR2(65)       | Not Null             | No   | No   |
| **LOV_SORT_POSITION_NUMBER** | Which position to display this itme in a drop-down list.  i.e. 1,2,3,....                                                | INTEGER            | Null                 | No   | No   |
| **LOV_LANGUAGE_DESC**        | Specifies which language to display the code in.  Note: this is not used in AML 2.1.  Will be removed in future release. | VARCHAR2(20)       | Null                 | No   | No   |

[Back to index](./index.md)