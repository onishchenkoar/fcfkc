# FSK_UI_AVAILABILITY

---

Used to indicate if the user interface is available - meaning the batch run has finished and it is now safe to use the

[Back to index](./index.md)

| Column Name                          | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **SEGMENT_ID**                       | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **UI_AVAILABILITY_IND APPLICATION.** | Is the user interface available for use Y/N.                                           | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)