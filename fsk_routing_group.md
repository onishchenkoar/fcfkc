# FSK_ROUTING_GROUP

---

A collection of user-defined routing rules that determine how an alert should initially be routed.

[Back to index](./index.md)

| Column Name            | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ROUTING_GROUP_ID**   | Unique identifier.                                                                     | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**         | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **ROUTING_GROUP_NAME** | Unique name for the group.                                                             | VARCHAR2(50)       | Not Null             | No   | No   |
| **LOGICAL_DELETE_IND** | Has this record been logically deleted Y/N.                                            | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)