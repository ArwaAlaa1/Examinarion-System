Project Title:
Examination System Database 📚

Project Description:
The Examination System Database is a comprehensive SQL Server-based project designed to manage and automate the process of creating, scheduling, and evaluating exams for educational institutions. 🏫 The system allows instructors to create exams from a pool of questions, manage courses, and evaluate student performance. It also provides functionalities for training managers to manage branches, tracks, and student information. The system supports multiple question types, including multiple-choice, true/false, and text-based questions, with automated grading for objective questions and manual review for text-based answers. 🖋️

Key Features:
Question Pool Management:

Store and manage a pool of questions (multiple-choice, true/false, and text-based). 📝

Allow instructors to select questions manually or randomly for exams. 🎲

Exam Creation and Scheduling:

Instructors can create exams for their courses, assign scores to questions, and ensure the total score does not exceed the course's maximum degree. 📊

Define exam details such as type (regular or corrective), intake, branch, track, course, start time, end time, and duration. ⏰

Automated and Manual Grading:

Automatically grade multiple-choice and true/false questions. ✅

Use text functions and regular expressions to evaluate text-based answers, with manual review and grading by instructors. 📄

Course and User Management:

Store course information (name, description, max degree, min degree). 📖

Manage instructor and student information. 👨‍🏫👩‍🎓

Assign instructors to courses and classes. 🏷️

Training Manager Functionalities:

Add and edit branches, tracks, and intakes. 🏢

Add students and define their personal data, intake, branch, and track. 📋

User Authentication:

Provide login accounts for training managers, instructors, and students. 🔐

Restrict access based on user roles. 🛡️

Student Exam Access:

Students can only access and take exams during the specified time. ⏳

Store student answers and calculate final results. 📊

Data Testing and Validation:

Insert test data into all tables to ensure system functionality. 🧪

Validate data integrity and consistency. ✔️

Database Schema Overview:
The database consists of the following main tables:

Courses:

Stores course information (CourseID, CourseName, Description, MaxDegree, MinDegree). 📚

Instructors:

Stores instructor details (InstructorID, Name, Email, etc.). 👨‍🏫

Students:

Stores student details (StudentID, Name, Intake, Branch, Track, etc.). 👩‍🎓

Questions:

Stores questions (QuestionID, QuestionText, Type, CorrectAnswer, CourseID). ❓

Exams:

Stores exam details (ExamID, ExamType, CourseID, InstructorID, StartTime, EndTime, TotalTime). 📅

StudentAnswers:

Stores student answers (AnswerID, StudentID, ExamID, QuestionID, Answer, Marks). 📝

Results:

Stores final results (ResultID, StudentID, CourseID, TotalMarks). 📊

Branches, Tracks, and Intakes:

Stores branch, track, and intake details managed by the training manager. 🏢

Setup Instructions:
Prerequisites:

SQL Server installed and running. 🖥️

SQL Server Management Studio (SSMS) or any compatible database management tool. 🛠️

Database Creation:

Run the provided SQL scripts to create the database, tables, and relationships. 🗃️

Ensure all constraints (primary keys, foreign keys, etc.) are applied. 🔗

Insert Test Data:

Use the provided test data scripts to populate the tables with sample data. 🧪

Verify that the data is correctly inserted and relationships are maintained. ✔️

User Authentication Setup:

Implement login functionality for training managers, instructors, and students. 🔐

Use stored procedures or application-level logic to handle user roles and permissions. 🛡️

Files Included:
SQL Scripts:

CreateDatabase.sql: Script to create the database. 🗃️

DDL.sql: Script to create Tables, Rules, User-defined data types, and Schemas. 📄

DML.sql: Script to insert sample data into the tables. 📝

DCL.sql: Script to create Accounts and Add Permissions for users. 🔐

StoredProcedures.sql: Script to create stored procedures for common operations. 🔄

Functions.sql: Script to create Functions for common operations. 🔧

Indexes.sql: Script to create Indexes for common columns. 📑

Views.sql: Script to create Views for common scenarios. 👀

Trigger.sql: Script to create triggers to ensure data integrity and users' access. 🚨

ER Diagram:

A visual representation of the database schema. 🗺️

Mapping Diagram:

A diagram showing the relationships between tables. 🔗

Assumptions:
