# FSK_UI_TABLE

---

Attribute Name :   table_ui_name

[Back to index](./index.md)

| Column Name                 | Column Definition                                                                            | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------------|:---------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **TABLE_UI_NAME**           | The name of the table.                                                                       | VARCHAR2(35)       | Not Null             | Yes  | No   |
| **TABLE_EXPRESSION_TEXT**   | Physical table name or SQL statement used to get the table.                                  | VARCHAR2(2000)     | Null                 | No   | No   |
| **TABLE_LABEL_DESC**        | Readable table name for display on the screen.                                               | VARCHAR2(64)       | Null                 | No   | No   |
| **TABLE_DATA_SOURCE_CODE**  | Values: COR or CTR                                                                           | CHAR(3)            | Null                 | No   | No   |
| **TABLE_SEARCH_LEVEL_CODE** | Level of information needed to display this table in the search query builder (LIT/BAS/EXT). | CHAR(3)            | Null                 | No   | No   |
| **TABLE_ACTIVE_IND**        | Is this table still active (Y/N) i.e. is it available to be displayed.                       | CHAR(1)            | Null                 | No   | No   |

[Back to index](./index.md)