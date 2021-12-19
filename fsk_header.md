# FSK_HEADER

---

Attribute Name :   header_id

[Back to index](./index.md)

| Column Name              | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **HEADER_ID**            | Name and identifier of the header.                                                     | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**           | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **HEADER_NAME**          | Short name for the header.                                                             | VARCHAR2(32)       | Not Null             | No   | No   |
| **HEADER_DESCRIPTION**   | Header description                                                                     | VARCHAR2(255)      | Not Null             | No   | No   |
| **ENTITY_LEVEL_CODE**    | Which entity level the header targets i.e. ACC, PTY, HHD, ASC.                         | CHAR(3)            | Not Null             | No   | No   |
| **DENORM_TABLE_NAME**    | Name of the denormalized table used as input to the Datastep code.                     | VARCHAR2(32)       | Null                 | No   | No   |
| **ALERT_TABLE_NAME**     | Location of intermediate alerts????                                                    | VARCHAR2(24)       | Not Null             | No   | No   |
| **HEADER_AUTOGEN_IND**   | Is the header autogen'd Y/N                                                            | CHAR(1)            | Not Null             | No   | No   |
| **HEADER_LOCATION_DESC** | Where is the header physically stored?                                                 | VARCHAR2(255)      | Null                 | No   | No   |
| **SOURCE_TYPE_DESC**     | e.g. SAS Datastep                                                                      | VARCHAR2(32)       | Not Null             | No   | No   |
| **CREATE_USER_ID**       | Who created the header.                                                                | VARCHAR2(60)       | Not Null             | No   | No   |
| **CREATE_DATE**          | When the header was created.                                                           | DATE               | Not Null             | No   | No   |
| **LSTUPDATE_USER_ID**    | Who last updated the header.                                                           | VARCHAR2(60)       | Null                 | No   | No   |
| **LSTUPDATE_DATE**       | When was the header last updated.                                                      | DATE               | Null                 | No   | No   |
| **HEADER_HOST_DESC**     | Whether running LOCALHOST or REMOTE.                                                   | VARCHAR2(50)       | Not Null             | No   | No   |
| **LOGICAL_DELETE_IND**   | Has this row been logically deleted Y/N                                                | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)