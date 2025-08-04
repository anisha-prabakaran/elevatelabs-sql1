# Elevate Labs - SQL Intern Task 1
## 📚 Task 1: Database Setup and Schema Design

### 🎯 Objective
To create a well-structured database schema by:
- Designing entities and their relationships
- Implementing the schema using SQL
- Generating an ER diagram

### 🛠️ Tools Used
- **MySQL Workbench**
- SQL

---

## Domain: Library Management System 📖

### Entities and Relationships

#### Entities:
1. **Author**
2. **Book**
3. **Member**
4. **Borrow**

#### Relationships:
- Each **Book** is written by one **Author**
- Each **Member** can borrow many **Books**
- Each **Borrow** record links a **Book** to a **Member**

---

## Database Schema

### ER Diagram

- The ER diagram for this schema has been uploaded as:  
  📄 **ER.pdf**  
  (Check the repository files)

### Tables & Relationships:

| Table Name | Primary Key | Foreign Keys |
|------------|-------------|--------------|
| Author     | AuthorID    | -            |
| Book       | BookID      | AuthorID → Author(AuthorID) |
| Member     | MemberID    | -            |
| Borrow     | BorrowID    | BookID → Book(BookID), MemberID → Member(MemberID) |



- The full SQL script to create the database schema has been uploaded 
