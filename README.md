College Database Management System
README
## Project Overview ##
This project is a College Database Management System implemented using Oracle SQL.
It is designed to manage and store data related to departments, students, faculty, courses, and course enrollment.
The database structure is based on an ER diagram which shows entities, attributes, and relationships clearly.
## Technologies Used ##
Database: Oracle SQL
Language: SQL
ER Diagram Tool: draw.io
## Database Tables Description ##
1.Dept_Master
This table stores department information.
Attributes:
Dept_ID (Primary Key)
Dept_Name
Office_Location
2.Student_Details
This table stores student information.
Attributes:
Student_ID (Primary Key)
Student_Name
Date_of_Birth
Gender
Contact_Number
Dept_ID (Foreign Key references Dept_Master)
3.Faculty_Details
This table stores faculty information.
Attributes:
Faculty_ID (Primary Key)
Faculty_Name
Designation
Email
Dept_ID (Foreign Key references Dept_Master)
4.Course_Details
This table stores course information.
Attributes:
Course_ID (Primary Key)
Course_Name
Credits
Dept_ID (Foreign Key references Dept_Master)
Faculty_ID (Foreign Key references Faculty_Details)
5.Course_Enrollment
This table manages enrollment of students in courses.
## Attributes:##
Enrollment_ID (Primary Key)
Student_ID (Foreign Key references Student_Details)
Course_ID (Foreign Key references Course_Details)
Semester
Grade
## Entity Relationships ##
One department can have many students, faculty members, and courses.
One faculty member can teach multiple courses.
One student can enroll in multiple courses.
The many-to-many relationship between students and courses is resolved using the Course_Enrollment table.
## ER Diagram ##
The ER diagram represents all entities, their attributes, primary keys, foreign keys, and relationships with proper cardinality.
The diagram is created using draw.io.

