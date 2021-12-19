# FSK_ERROR_LOG

---

Attribute Name :   stored_procedure_name

[Back to index](./index.md)

| Column Name               | Column Definition                        | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------------|:-----------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **STORED_PROCEDURE_NAME** | Teradata stored procedure scenario name. | VARCHAR2(35)       | Null                 | No   | No   |
| **CREATE_DATE**           | Date the error log record was created.   | DATE               | Null                 | No   | No   |
| **SQL_STATE**             | SQL state returned by the RDBMS.         | VARCHAR2(35)       | Null                 | No   | No   |
| **SQL_CODE**              | SQL code returned by the RDBMS.          | VARCHAR2(35)       | Null                 | No   | No   |
| **SQL_ERROR_MESSAGE**     | SQL error message returned by the RDBMS. | VARCHAR2(255)      | Null                 | No   | No   |

[Back to index](./index.md)