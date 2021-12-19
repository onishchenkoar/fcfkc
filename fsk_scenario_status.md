# FSK_SCENARIO_STATUS

---

Contains start and end time for each Teradata scenario execution.

[Back to index](./index.md)

| Column Name               | Column Definition                            | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------------|:---------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **STORED_PROCEDURE_NAME** | Teradata stored procedure scenario name.     | VARCHAR2(35)       | Null                 | No   | No   |
| **CREATE_DATE**           | Date the scenario status record was created. | DATE               | Null                 | No   | No   |
| **BEGIN_TIME**            | Stored procedure scenario start time.        | DATE               | Null                 | No   | No   |
| **END_TIME**              | Stored procedure scenario end time.          | DATE               | Null                 | No   | No   |

[Back to index](./index.md)