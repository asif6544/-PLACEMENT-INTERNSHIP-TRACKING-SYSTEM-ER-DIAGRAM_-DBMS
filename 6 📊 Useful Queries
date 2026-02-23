🔹 1. Show all students
SELECT * FROM Student;
🔹 2. Students with CGPA > 8
SELECT * FROM Student WHERE CGPA > 8;
🔹 3. Show drives with company name
SELECT d.Drive_ID, c.Company_Name, d.Job_Role, d.Package
FROM Placement_Drive d
JOIN Company c ON d.Company_ID = c.Company_ID;
🔹 4. Show student applications with status
SELECT s.Name, d.Job_Role, a.Status
FROM Application a
JOIN Student s ON a.Student_ID = s.Student_ID
JOIN Placement_Drive d ON a.Drive_ID = d.Drive_ID;
🔹 5. Show accepted offers
SELECT s.Name, c.Company_Name, o.Salary
FROM Offer o
JOIN Student s ON o.Student_ID = s.Student_ID
JOIN Company c ON o.Company_ID = c.Company_ID
WHERE o.Offer_Status = 'Accepted';
