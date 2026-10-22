# Gradebook Management System - Sections E&F
# Project Overview
The Gradebook Management System is a Python application designed to manage student academic records.
The system uses Object-Oriented Programming principles to organize student information and grade data.
It allows users to add, remove, search, sort and display student records while providing validation and exception handling to improve reliability and user experience.

The purpose of this system is to demonstrate the application of classes, objects, methods, exception handling, searching, sorting and testing techniques within a Gradebook environment.

# Setup Instructions
* Open the project in PyCharm or another Python IDE.
* Ensure Python is installed on your computer.
* Save the program as a Python file.
* Run the program using:
  python main.py or depending on the file name used.

# Features List
* Add student records.
* Store grades for Mathematics, English, and Science.
* Calculate student averages.
* Remove students from the system.
* Search for students by name.
* Display student details.
* Display all student records.
* Sort students by average grade.
* Sort students by subject grades.
* Validate student names.
* Validate grade ranges (0–100).
* Handle non-numeric grade input.
* Handle missing student records.
* Handle duplicate student names.
* Use custom exceptions for error handling.
* Test system functionality.
* Class Architecture
* Student Class, the Student class represents an individual student.

# Attributes

* name
* math
* english
* science
  
# Methods

* add_grades()
* calculate_average()
* display_student()

# Gradebook Class
The Gradebook class manages all student records.

# Attributes

students

# Methods

* get_name()
* get_grade()
* add_student()
* remove_student()
* search_student()
* sort_by_average()
* sort_by_subject()
* display_summary()
* test_system()
  
# Relationship

The Gradebook class stores and manages multiple Student objects.

Example Input/Output

Adding a Student

Input

Select an option: 1

Enter student name: Bosha

Enter Math grade (0-100): 85

Enter English grade (0-100): 80

Enter Science grade (0-100): 90

Output

Student added successfully.
Searching for a Student

Input

Select an option: 3

Enter student name to search: Bouh

Output

Name: John
Math: 85
English: 80
Science: 90
Average: 85.0
Invalid Grade Input

Input

Enter Math grade (0-100): abc

Output

Invalid input. Please enter a numeric grade.

# Assumptions and Limitations

# Assumptions

* Grades must be between 0 and 100.
* Student names must contain alphabetic characters.
* Mathematics, English and Science are the only supported subjects.
* Users interact with the program through the menu system.

# Limitations

* Data is not permanently stored after the program closes.

* Student records exist only while the program is running.

* The system uses a console-based interface.

# Testing Summary

# Test Case. Expected Result. Actual Result	Status

Add valid student. Student added successfully. Pass

Enter grade above 100. Grade rejected and re-prompted. Pass

Enter negative grade. Grade rejected and re-prompted.	Pass

Enter non-numeric grade. Error message displayed.	Pass

Search existing student. Student details displayed.	Pass

Search non-existent student. Student not found message. Pass

Remove existing student. Student removed.	Pass

Remove non-existent student.	Exception handled. Pass

Add duplicate student.	Duplicate rejected.	Pass

Sort by average.	Students sorted correctly.  Pass

Sort by subject.	Students Sorted correctly. Pass

# Edge Cases Tested

* Duplicate student names.
* Empty student names.
* Special character names (O'Neil, Jean-Pierre).
* Grades below 0.
* Grades above 100.
* Non-numeric grades.
* Searching for non-existent students.
* Removing non-existent students.
* Known Issues
* Student information is not saved to a file or database.
* Data is lost when the application closes.

# How They Were Addressed

* Input validation was added to reduce invalid entries.
* Exception handling was implemented to prevent the program from crashing when errors occur.

# References

Course Materials:

IDE: PyCharm

Programming Language: Python

Python Version: 3.14.7

No external libraries were used in the development of this project.

# License
This project was developed for educational purposes as part of a Python Programming continuous assessment.

All Rights Reserved.

# Contact
Maintainer: Bosha Phoebes Keorapetse

Institution: Botswana Accountancy College

For academic queries relating to this project, please contact the author through the appropriate course communication channels.
