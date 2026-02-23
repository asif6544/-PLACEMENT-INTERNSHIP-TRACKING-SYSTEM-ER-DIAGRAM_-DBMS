
📘 Placement & Internship Tracking System
👥 DBMS Group Project
📌 Project Overview

The Placement & Internship Tracking System is a Database Management System (DBMS) project designed to manage and track student internship and placement activities efficiently.

This system helps:

🎓 Students apply for internships and placements

🏢 Companies post internship and job opportunities

📊 Track application status (Selected / Rejected / Pending)

📁 Manage placement records in a structured database

🎯 Objectives

Design an ER Diagram with proper relationships

Convert ER model into relational schema

Implement database using SQL (MySQL)

Apply constraints (Primary Key, Foreign Key, Unique, etc.)

Ensure data integrity and normalization

🗂 Entities Used (5 Entities – 5 Attributes Each)
1️⃣ Student

Student_ID (PK)

Name

Department

Email

CGPA

2️⃣ Company

Company_ID (PK)

Company_Name

Industry_Type

Location

HR_Contact

3️⃣ Internship

Internship_ID (PK)

Internship_Role

Duration

Stipend

Company_ID (FK)

4️⃣ Placement

Placement_ID (PK)

Job_Role

Package

Placement_Date

Company_ID (FK)

5️⃣ Application

Application_ID (PK)

Application_Date

Status

Student_ID (FK)

Company_ID (FK)

🔗 Relationships

A Student applies for Applications (1:M)

An Application is sent_to Company (M:1)

A Company offers Internship (1:M)

A Company offers Placement (1:M)

🧱 Database Schema

All tables created using CREATE TABLE

Primary Keys defined for all entities

Foreign Keys implemented for relationships

Cascading rules applied for referential integrity

🛠 Technologies Used

💾 MySQL

📊 ER Diagram (Box & Diamond Style)

🧠 DBMS Concepts (Normalization, Constraints, Relationships)

💻 SQL Queries

📈 Features

✔ Student Registration
✔ Company Management
✔ Internship & Placement Tracking
✔ Application Status Management
✔ Data Integrity using Constraints

📊 Normalization

✔ 1NF – Atomic attributes

✔ 2NF – No partial dependency

✔ 3NF – No transitive dependency

Database is normalized up to Third Normal Form (3NF).

📂 Project Structure
📦 Placement-Internship-Tracking-System
 ┣ 📜 README.md
 ┣ 📜 ER_Diagram.png
 ┣ 📜 SQL_Schema.sql
 ┣ 📜 Sample_Data.sql
 ┗ 📜 Project_Report.pdf
👥 Group Members

Member 1 – Name

Member 2 – Name

Member 3 – Name

Member 4 – Name

(Add your team member names here)

🚀 How to Run

Install MySQL

Create a new database

Run the SQL schema file

Insert sample data

Execute SELECT queries

📚 Learning Outcomes

Practical understanding of ER modeling

Implementation of relational schema

Writing complex SQL queries

Understanding DBMS concepts in real-world scenarios

📌 Conclusion

This project demonstrates how DBMS can be used to manage real-world placement and internship processes efficiently. It improves data organization, tracking, and decision-making within an institution.
