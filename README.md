# 📘 Placement & Internship Tracking System  
### 👥 DBMS Group Project

---

## 📌 Project Overview

The **Placement & Internship Tracking System** is a Database Management System (DBMS) project designed to manage and track student internship and placement activities efficiently.

This system allows institutions to:

- Manage student information  
- Maintain company records  
- Track internship opportunities  
- Track placement offers  
- Monitor application status (Selected / Rejected / Pending)  

The database ensures structured data storage, integrity, and efficient retrieval of placement-related information.

---

## 🎯 Project Objectives

- Design an ER Diagram with 5 entities and 5 attributes each  
- Convert ER Model into Relational Schema  
- Implement database using SQL (MySQL)  
- Apply Primary Key and Foreign Key constraints  
- Maintain normalization up to Third Normal Form (3NF)  
- Ensure referential integrity  

---

## 🗂 Entities and Attributes

### 1️⃣ Student
- Student_ID (Primary Key)  
- Name  
- Department  
- Email  
- CGPA  

### 2️⃣ Company
- Company_ID (Primary Key)  
- Company_Name  
- Industry_Type  
- Location  
- HR_Contact  

### 3️⃣ Internship
- Internship_ID (Primary Key)  
- Internship_Role  
- Duration  
- Stipend  
- Company_ID (Foreign Key)  

### 4️⃣ Placement
- Placement_ID (Primary Key)  
- Job_Role  
- Package  
- Placement_Date  
- Company_ID (Foreign Key)  

### 5️⃣ Application
- Application_ID (Primary Key)  
- Application_Date  
- Status  
- Student_ID (Foreign Key)  
- Company_ID (Foreign Key)  

---

## 🔗 Relationships

- A Student applies for Applications (1:M)  
- An Application is sent to a Company (M:1)  
- A Company offers Internship (1:M)  
- A Company offers Placement (1:M)  

---

## 🧱 ER Diagram

The ER Diagram includes:

- Rectangles → Entities  
- Diamonds → Relationships  
- Ovals → Attributes  
- Underlined → Primary Keys  
- 1:M cardinality relationships  

(ER diagram image included in the repository)

---

## 🛠 Technologies Used

- MySQL  
- SQL  
- ER Modeling  
- DBMS Concepts  
- GitHub  

---

## 💾 Database Implementation

- All tables created using `CREATE TABLE`
- Primary Keys defined for each entity
- Foreign Keys used to maintain relationships
- Constraints applied to maintain data consistency
- Database normalized up to 3NF

---

## 📊 Features

- Student registration management  
- Company information management  
- Internship tracking  
- Placement tracking  
- Application status monitoring  
- Data integrity using constraints  

---

## 📁 Project Structure
Placement-Internship-Tracking-System/
/README.md
  ER_Diagram.png
  SQL_Schema.sql
  Sample_Data.sql
  Project_Report.pdf


---

## 👥 Group Members

- Member 1 – MD ASIF
- Member 2 – Kunal Agratam
- Member 3 – Manish Singh 
- Member 4 – Manas

---

## 🚀 How to Run

1. Install MySQL  
2. Create a new database  
3. Execute the SQL schema file  
4. Insert sample data  
5. Run SELECT queries to view results  

---

## 📚 Learning Outcomes

- Understanding ER Diagram design  
- Converting ER model to relational schema  
- Writing SQL queries  
- Applying normalization concepts  
- Implementing database constraints  

---

## 📌 Conclusion

The Placement & Internship Tracking System demonstrates the practical implementation of DBMS concepts in managing real-world placement processes. The system ensures organized data management, consistency, and efficient tracking of internships and placements.

---

⭐ Thank you for viewing our DBMS Group Project!
