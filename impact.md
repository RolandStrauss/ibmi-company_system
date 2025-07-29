
## Project Listing

<details><summary>Click to expand</summary><br>

| - | Object | Type | Path | Warnings | Parents | Children |
| --- | --- | --- | --- | --- | --- | --- |
| 📁 | DEPTS | FILE | `qddssrc\depts.dspf` | ✅ | <details><summary>1</summary>DEPTS.PGM</details> | 0 |
| 📁 | EMPS | FILE | `qddssrc\emps.dspf` | ✅ | <details><summary>1</summary>EMPLOYEES.PGM</details> | 0 |
| 📁 | NEMP | FILE | `qddssrc\nemp.dspf` | ✅ | <details><summary>1</summary>NEWEMP.PGM</details> | 0 |
| 📒 | APP | BNDDIR | `qrpglesrc\app.bnddir` | ✅ | 0 | <details><summary>1</summary>EMPDET.SRVPGM</details> |
| 🛠️ | DEPTS | PGM | `qrpglesrc\depts.pgm.sqlrpgle` | ✅ | 0 | <details><summary>4</summary>EMPLOYEES.PGM, NEWEMP.PGM, DEPARTMENT.FILE, DEPTS.FILE</details> |
| 📦 | EMPDET | SRVPGM | `qrpglesrc\empdet.bnd` | ✅ | <details><summary>1</summary>APP.BNDDIR</details> | <details><summary>1</summary>EMPDET.MODULE</details> |
| ⛏️ | EMPDET | MODULE | `qrpglesrc\empdet.sqlrpgle` | ✅ | <details><summary>1</summary>EMPDET.SRVPGM</details> | <details><summary>2</summary>EMPLOYEE.FILE, DEPARTMENT.FILE</details> |
| 🛠️ | EMPLOYEES | PGM | `qrpglesrc\employees.pgm.sqlrpgle` | <details><summary>ℹ️</summary><br>has the BNDDIR keyword. Binding directory should be set at global level or object level.</details> | <details><summary>1</summary>DEPTS.PGM</details> | <details><summary>2</summary>EMPLOYEE.FILE, EMPS.FILE</details> |
| 🛠️ | MYPGM | PGM | `qrpglesrc\mypgm.pgm.rpgle` | ✅ | 0 | 0 |
| 🛠️ | NEWEMP | PGM | `qrpglesrc\newemp.pgm.sqlrpgle` | ✅ | <details><summary>1</summary>DEPTS.PGM</details> | <details><summary>2</summary>EMPLOYEE.FILE, NEMP.FILE</details> |
| ⛏️ | TEMPDET | MODULE | `qtestsrc\empdet.test.sqlrpgle` | <details><summary>ℹ️</summary><br>has the BNDDIR keyword. Binding directory should be set at global level or object level.</details> | 0 | <details><summary>2</summary>EMPLOYEE.FILE, DEPARTMENT.FILE</details> |
| 📁 | EMPLOYEE | FILE | `qsqlsrc\employee.table` | <details><summary>ℹ️</summary><br>EMPLOYEE (TABLE) alter not tracked due to possible circular dependency.</details> | <details><summary>5</summary>EMPDET.MODULE, EMPLOYEES.PGM, NEWEMP.PGM, POPEMP.PGM, TEMPDET.MODULE</details> | 0 |
| 🛠️ | POPDEPT | PGM | `qsqlsrc\popdept.sqlprc` | ✅ | 0 | <details><summary>1</summary>DEPARTMENT.FILE</details> |
| 🛠️ | POPEMP | PGM | `qsqlsrc\popemp.sqlprc` | ✅ | 0 | <details><summary>2</summary>EMPLOYEE.FILE, DEPARTMENT.FILE</details> |
| 📁 | DEPARTMENT | FILE | `qsqlsrc\department.table` | <details><summary>ℹ️</summary><br>DEPARTMENT (TABLE) alter not tracked due to possible circular dependency.</details> | <details><summary>5</summary>EMPDET.MODULE, DEPTS.PGM, POPEMP.PGM, POPDEPT.PGM, TEMPDET.MODULE</details> | 0 |

* *Parents* are objects that depend on this object.
* *Children* are objects that this object depends on.

</details>
