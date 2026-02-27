-- =========================================
-- Internship Placement Database
-- =========================================

-- 1️⃣ Create Database
CREATE DATABASE Internship_Placement_DB;
USE Internship_Placement_DB;

-- =========================================
-- 2️⃣ Student Table
-- =========================================
CREATE TABLE Student (
    Student_ID INT PRIMARY KEY,
    Name VARCHAR(100) NOT NULL,
    Email VARCHAR(100) UNIQUE,
    CGPA DECIMAL(3,2),
    Department VARCHAR(100)
);

-- =========================================
-- 3️⃣ Company Table
-- =========================================
CREATE TABLE Company (
    Company_ID INT PRIMARY KEY,
    Company_Name VARCHAR(150) NOT NULL,
    Industry_Type VARCHAR(100),
    Location VARCHAR(100),
    HR_Contact VARCHAR(100)
);

-- =========================================
-- 4️⃣ Internship Table
-- One Company → Many Internships
-- =========================================
CREATE TABLE Internship (
    Internship_ID INT PRIMARY KEY,
    Company_ID INT NOT NULL,
    Internship_Role VARCHAR(100),
    Duration VARCHAR(50),
    Stipend DECIMAL(10,2),
    FOREIGN KEY (Company_ID)
        REFERENCES Company(Company_ID)
        ON DELETE CASCADE
);

-- =========================================
-- 5️⃣ Placement Table
-- One Student → Many Placements
-- One Internship → Many Placements
-- =========================================
CREATE TABLE Placement (
    Placement_ID INT PRIMARY KEY,
    Student_ID INT NOT NULL,
    Internship_ID INT NOT NULL,
    Date_of_Selection DATE,
    Status VARCHAR(50),
    Final_Result VARCHAR(50),
    FOREIGN KEY (Student_ID)
        REFERENCES Student(Student_ID)
        ON DELETE CASCADE,
    FOREIGN KEY (Internship_ID)
        REFERENCES Internship(Internship_ID)
        ON DELETE CASCADE
);

-- =========================================
-- 6️⃣ Interview Table
-- One Placement → Many Interviews
-- =========================================
CREATE TABLE Interview (
    Interview_ID INT PRIMARY KEY,
    Placement_ID INT NOT NULL,
    Interview_Date DATE,
    Round_Type VARCHAR(50),
    Result VARCHAR(50),
    FOREIGN KEY (Placement_ID)
        REFERENCES Placement(Placement_ID)
        ON DELETE CASCADE
);

-- =========================================
-- End of File
-- =========================================
