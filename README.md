SEN 201 TASK
Name: Rukeme Ekpiteta Jnr
Martic no: 24/14894
Department: computer science
Part A: Student Result Management System (SRMS)
1. Introduction
The Student Result Management System (SRMS) is a simple software application designed to store, 
calculate, and display students’ academic results. It reduces manual errors, saves time, and improves
efficiency in result processing.
2 Requirement Analysis
Functional Requirements:
 Add student name
 Add student score
 Calculate grade
 Display student result
Non-Functional Requirements:
 Easy to use
 Fast execution
 Runs on any system with Python installed
2.2 System Design
Program Structure:
 Student_name
 student_score
 grade
 calculate_grade() function
 display_result() function  60 – 69 → B
 50 – 59 → C
 45 – 49 → D
 Below 45 → F
Note: These names are used exactly in the implementation.
2.3 Implementation
Create a file named:
student_result_management_system.py
Code:
def calculate_grade(student_score):
 if student_score >= 70:
 return "A"
 elif student_score >= 60:
 return "B"
 elif student_score >= 50:
 return "C"
 elif student_score >= 45:
 return "D"
 else:
 return "F"
def display_result(student_name, student_score, grade):
 print("\n--- Student Result ---")
 print("Name:", student_name)
 print("Score:", student_score)
 print("Grade:", grade)
# Main Program student_name = input("Enter student name: ")
student_score = int(input("Enter student score: "))
grade = calculate_grade(student_score)
display_result(student_name, student_score, grade)

