# 🗄️ Database - Basics
> IT Student Notes | Topic: Database Fundamentals

---

## 📌 Table of Contents
1. [Database Kya Hai](#1-database-kya-hai)
2. [DBMS Kya Hai](#2-dbms-kya-hai)
3. [Types of Databases](#3-types-of-databases)
4. [Table, Row, Column](#4-table-row-column)
5. [Important Terms](#5-important-terms)
6. [SQL Basics](#6-sql-basics)
7. [CRUD Operations](#7-crud-operations)
8. [Quick Revision](#8-quick-revision)

---

## 1. Database Kya Hai

- Data ko **organized way** mein store karna
- Easily **search, update, delete** kar sako
- Example: School ka student record, Bank ka account data

### File System vs Database:

| | File System | Database |
|--|-------------|---------|
| Storage | Random files | Organized tables |
| Search | Mushkil ❌ | Easy ✅ |
| Duplication | Hoti hai | Nahi hoti ✅ |
| Security | Weak | Strong ✅ |
| Example | .txt, .csv files | MySQL, Oracle |

---

## 2. DBMS Kya Hai

- DBMS = **Database Management System**
- Software jo database manage karta hai

```
User → DBMS → Database
         ↓
   Data store/retrieve/update/delete
```

### Popular DBMS:

| DBMS | Type | Use |
|------|------|-----|
| **MySQL** | Relational | Web apps ✅ |
| **Oracle** | Relational | Enterprise |
| **PostgreSQL** | Relational | Advanced apps ✅ |
| **MongoDB** | NoSQL | Flexible data |
| **SQLite** | Relational | Small apps |
| **Redis** | NoSQL | Fast caching |

---

## 3. Types of Databases

### Relational Database (SQL):
- Data **tables** mein store hota hai
- Tables ke beech **relations** hoti hain
- SQL language use hoti hai

```
Students Table ←→ Marks Table ←→ Courses Table
(Related hain!)
```

### NoSQL Database:
- **Flexible structure** hoti hai
- Tables ki zaroorat nahi
- JSON jaisa format

```
{
  "id": 1,
  "name": "Rahul",
  "marks": 85
}
```

### Relational vs NoSQL:

| | Relational | NoSQL |
|--|------------|-------|
| Structure | Fixed tables | Flexible |
| Language | SQL | Varies |
| Scale | Vertical | Horizontal ✅ |
| Use | Banking, ERP | Social media, BigData |
| Example | MySQL | MongoDB |

---

## 4. Table, Row, Column

```
STUDENTS Table:

| ID | Name    | Age | Marks |
|----|---------|-----|-------|
| 1  | Rahul   | 20  | 85    |
| 2  | Priya   | 21  | 90    |
| 3  | Amit    | 20  | 78    |

Row    = Ek student ka poora record (horizontal)
Column = Ek property (vertical) - Name, Age, Marks
Cell   = Ek value - "Rahul", 85
```

---

## 5. Important Terms

| Term | Matlab | Example |
|------|--------|---------|
| **Table** | Data rows aur columns mein | Students table |
| **Row/Record** | Ek entry | Ek student ka data |
| **Column/Field** | Ek property | Name, Age, Marks |
| **Primary Key** | Unique identifier | ID (har row ka alag) |
| **Foreign Key** | Doosri table se link | Course_ID |
| **Query** | Database se data maangna | SELECT * FROM... |
| **Schema** | Database ka structure | Tables ka design |
| **Index** | Fast search ke liye | Primary key pe auto |

### Primary Key:
```
Primary Key = Har row ka unique identifier

| ID | Name  |   ← ID = Primary Key
|----|-------|     (Koi 2 rows ka ID same nahi hoga)
| 1  | Rahul |
| 2  | Priya |
| 3  | Amit  |
```

### Foreign Key:
```
STUDENTS Table:        COURSES Table:
| ID | Name  | C_ID |  | C_ID | Course   |
|----|-------|------|  |------|----------|
| 1  | Rahul | 101  |  | 101  | IT       |
| 2  | Priya | 102  |  | 102  | CS       |
        ↑                  ↑
   Foreign Key ────────→ Primary Key
```

---

## 6. SQL Basics

- SQL = **Structured Query Language**
- Database se **baat** karne ki language

### Data Dekhna (SELECT):
```sql
-- Saari rows dekhna
SELECT * FROM students;

-- Specific columns
SELECT name, marks FROM students;

-- Condition ke saath
SELECT * FROM students WHERE marks > 80;

-- Order mein
SELECT * FROM students ORDER BY marks DESC;
```

### Data Add Karna (INSERT):
```sql
INSERT INTO students (id, name, age, marks)
VALUES (4, 'Neha', 21, 92);
```

### Data Update Karna (UPDATE):
```sql
UPDATE students
SET marks = 95
WHERE id = 1;
```

### Data Delete Karna (DELETE):
```sql
DELETE FROM students
WHERE id = 3;
```

### Table Banana (CREATE):
```sql
CREATE TABLE students (
    id      INT PRIMARY KEY,
    name    VARCHAR(50),
    age     INT,
    marks   FLOAT
);
```

---

## 7. CRUD Operations

```
C → Create  → INSERT  → Naya data add karo
R → Read    → SELECT  → Data dekhna
U → Update  → UPDATE  → Data change karo
D → Delete  → DELETE  → Data hatao
```

| Operation | SQL Command | Example |
|-----------|-------------|---------|
| **Create** | INSERT | Naya student add |
| **Read** | SELECT | Student list dekhna |
| **Update** | UPDATE | Marks change karna |
| **Delete** | DELETE | Student remove karna |

---

## 8. Quick Revision

```
Database  = Organized data store
DBMS      = Database manage karne ka software
MySQL     = Popular relational DBMS ✅
Table     = Rows + Columns mein data
Row       = Ek record (ek student)
Column    = Ek property (name, age)
Primary Key = Unique row identifier
Foreign Key = Doosri table se link
SQL       = Database ki language
CRUD      = Create, Read, Update, Delete
```

### SQL Commands Summary:
```sql
SELECT  → Data read karo
INSERT  → Data add karo
UPDATE  → Data change karo
DELETE  → Data hatao
CREATE  → Table banao
DROP    → Table hatao
```

---

*Notes by: IT Student*
*Topic: Database - Basics*
