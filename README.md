📘 Student Result Management System (Java)
🧩 Project Overview

The Student Result Management System is a console-based Java application designed to collect student details, validate marks, calculate results, and display student performance.
It demonstrates robust exception handling in Java using try-catch-finally, throw, throws, and custom exceptions.

🎯 Objectives

Implement Java Exception Handling in a real-world scenario.

Differentiate between checked and unchecked exceptions.

Create and use custom exception classes (InvalidMarksException).

Use try, catch, throw, throws, and finally effectively.

Ensure robust and user-friendly program execution.

🏗️ Class Structure
1. InvalidMarksException

Custom checked exception extending Exception.

Thrown when marks are outside the range 0–100.

Provides meaningful error messages.

2. Student

Attributes:

rollNumber (Integer)

studentName (String)

marks (Integer[3])

Methods:

validateMarks() → Validates marks between 0–100.

calculateAverage() → Returns average of three subjects.

displayResult() → Displays student details and result status (Pass/Fail).

Throws InvalidMarksException for invalid input.

3. ResultManager

Handles all user interaction and exception handling.

Attributes:

Array of Student objects.

Scanner object for user input.

Methods:

addStudent() → Adds new student details after validation.

showStudentDetails() → Displays result for a specific student.

mainMenu() → Provides menu-driven interface.

Uses try-catch-finally for robust program control.

🧠 Exception Handling Demonstrated
Type	Example
Checked Exception	InvalidMarksException (custom)
Unchecked Exception	InputMismatchException, IllegalArgumentException
throw	Used in validateMarks() and constructor to raise exceptions
throws	Declared in methods that might throw checked exceptions
finally	Used to safely close the Scanner object
🖥️ Sample Interaction
===== Student Result Management System =====
1. Add Student
2. Show Student Details
3. Exit
Enter your choice: 1
Enter Roll Number: 101
Enter Student Name: Alice
Enter marks for subject 1: 85
Enter marks for subject 2: 92
Enter marks for subject 3: 88
Student added successfully. Returning to main menu...

===== Student Result Management System =====
1. Add Student
2. Show Student Details
3. Exit
Enter your choice: 2
Enter Roll Number to search: 101
Roll Number: 101
Student Name: Alice
Marks: 85 92 88
Average: 88.33333333333333
Result: Pass
Search completed.

===== Student Result Management System =====
1. Add Student
2. Show Student Details
3. Exit
Enter your choice: 3
Exiting program. Thank you!
Scanner closed. Program terminated.

⚠️ Error Handling Example
Enter Roll Number: 102
Enter Student Name: Bob
Enter marks for subject 1: -10
Error: Invalid marks for subject 1: -10. Allowed range is 0 to 100.
Returning to main menu...

🧩 Concepts Practiced

Object-Oriented Programming (OOP)

Exception Handling (try, catch, finally)

Custom Exceptions (InvalidMarksException)

Input validation and error messages

Array-based data storage

Console-based user interface

🛠️ How to Run

Save the code as ResultManager.java.

Open the terminal or command prompt in the project directory.

Compile the program:

javac ResultManager.java


Run the program:

java ResultManager

📚 Learning Outcomes

Understand and apply exception handling effectively in Java.

Differentiate between checked and unchecked exceptions.

Design custom exception classes for validation.

Build clean, modular, and error-resilient Java programs.

👩‍💻 Developed By

Lakshita Kalra
B.Tech CSE – K.R. Mangalam University
