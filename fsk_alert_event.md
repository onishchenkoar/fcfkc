# FSK_ALERT_EVENT

---

Attribute Name :   event_id

[Back to index](./index.md)

| Column Name           | Column Definition                                                                         | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------|:------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **EVENT_ID**          | A system generated synthetic key used to uniquely identify an instance of an alert event. | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**        | Multibank configurations use this column to indicate which bank the record belongs to.    | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **ALERT_ID**          | System generated synthetic/surrogate key that uniquely identifies an alert.               | NUMBER(12)         | Not Null             | No   | Yes  |
| **EVENT_TYPE_CODE**   | Describes whether the event was for example: "Alert Checked In", "Alert Checked Out" etc. | CHAR(3)            | Not Null             | No   | No   |
| **EVENT_DESCRIPTION** | Free-form description of the event.                                                       | VARCHAR2(255)      | Null                 | No   | No   |
| **CREATE_DATE**       | Date the record was created.                                                              | DATE               | Not Null             | No   | No   |
| **CREATE_USER_ID**    | Who created the record.                                                                   | VARCHAR2(60)       | Not Null             | No   | No   |

[Back to index](./index.md)