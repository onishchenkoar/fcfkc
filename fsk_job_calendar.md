# FSK_JOB_CALENDAR

---

Attribute Name :   job_calendar_id

[Back to index](./index.md)

| Column Name             | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **JOB_CALENDAR_ID**     | System generated surrogate key.                                                        | NUMBER(5)          | Not Null             | Yes  | No   |
| **SEGMENT_ID**          | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **CALENDAR_DATE**       | Calendar Date.                                                                         | DATE               | Null                 | No   | No   |
| **RUNDATE_IND**         | Is today a rundate regardless of type.                                                 | CHAR(1)            | Null                 | No   | No   |
| **DAILY_RUNDATE_IND**   | Do daily jobs run on this day? Y/N                                                     | CHAR(1)            | Not Null             | No   | No   |
| **WEEKLY_RUNDATE_IND**  | Do weekly jobs run on this day? Y/N                                                    | CHAR(1)            | Not Null             | No   | No   |
| **MONTHLY_RUNDATE_IND** | Do monthly jobs run on this day? Y/N                                                   | CHAR(1)            | Not Null             | No   | No   |
| **STATUS_IND**          | Have the jobs completed for this day?                                                  | CHAR(1)            | Not Null             | No   | No   |
| **BUSINESS_DAY_COUNT**  | A sequential number used to track business days versus holidays or weekends.           | NUMBER(15)         | Null                 | No   | No   |

[Back to index](./index.md)