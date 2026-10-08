# Student Management System Using MongoDB

A NoSQL mini project demonstrating core MongoDB operations on a collection of 30 student records, run in **mongosh**.

## Project Details

| | |
|---|---|
| University | Babu Banarasi Das University (2026-2027) |
| School | School of Computer Applications |
| Department | BCA (DS & AI) |
| Submitted by | Devmangal Gupta |
| Roll No | 23 |
| University Roll No | 1250258184 |
| Section | BCADS23 |
| Submitted to | Mr. Harendra Singh |

## Overview

The project creates a `Students` database with a `students` collection. Each document stores a student's roll number, name, age, marks and city. The queries cover CRUD operations, comparison and logical operators, sorting, limiting and counting.

## Document Structure

```js
{
  roll: 101,
  name: "Shrishti Singh",
  age: 19,
  marks: 85,
  city: "Delhi"
}
```

## Repository Contents

| File | Description |
|---|---|
| `README.md` | Project overview and usage instructions |
| `dataset.pdf` | All 30 student records and the `insertMany` script |
| `queries.pdf` | All 18 MongoDB queries with explanations |
| `No_sql_Project.pdf` | Full project report with output screenshots |

## Operations Covered

| Category | Operations |
|---|---|
| Database / Collection | `use`, `createCollection` |
| Create | `insertMany` |
| Read | `find`, `countDocuments`, `limit`, `sort` |
| Update | `updateOne` with `$set` |
| Delete | `deleteOne`, `deleteMany` |
| Comparison operators | `$eq`, `$gt`, `$lt`, `$gte`, `$lte` |
| Logical operators | `$and`, `$or` |

## How to Run

1. Install MongoDB and `mongosh`.
2. Start the MongoDB server and open `mongosh`.
3. Run the commands from `queries.pdf` in order, using the data from `dataset.pdf` for the insert step.

```js
use Students
db.createCollection("students")
db.students.find()
```

## Note on Results

Query 10 changes roll 105's marks to 95. Queries 11 and 12 delete records (roll 110, then rolls 111 and 113), so the collection holds **27 documents** at the end.

## Technologies Used

- MongoDB
- mongosh (MongoDB Shell)
