# PYTHON-LAB-1-GROUP-3-
-------Student Management and Text Processing Python Project----
Group Members:
Member 1: NISHIMWE Diane 26314
Member 2: ISHIMWE Esther 27751
Member 3: SHINGIRO Faisal 26499
Member 4: NIYONIZEYE Gabin 26653
Member 5: RWAGAPFIZI Igor  27329
Member 6: MUNYEMANA Honore 25594


Project Overview:
This project is a Python-based console application designed to demonstrate practical programming skills in student information management, palindrome checking, and text processing. The project is structured into three separate solutions, each addressing a specific task.

Activities and Solutions:
Answer 1: Student Management System
This solution captures student details, calculates the average grade, and displays the complete student information.

Key Features:
Inputs student name, age, number of courses, and grades.

Calculates the average grade from the provided courses.

Displays a detailed summary of the student's information.
............................................................................................................................
# Function to input student information
def input_student_info():
    name = input("Enter student name: ")
    age = int(input("Enter student age: "))
    num_courses = int(input("Enter number of courses (2 or 3): "))
    grades = []
    for i in range(num_courses):
        grade = float(input(f"Enter grade for course {i+1}: "))
        grades.append(grade)
    return name, age, grades

# Function to calculate average grade
def calculate_average(grades):
    return sum(grades) / len(grades)

# Function to display student information
def display_student_info(name, age, average):
    print("\n--- Student Information ---")
    print(f"Name: {name}")
    print(f"Age: {age}")
    print(f"Average Grade: {average:.2f}")

# Main function to run the student management system
def student_management_system():
    name, age, grades = input_student_info()
    average = calculate_average(grades)
    display_student_info(name, age, average)

# Call the main function
student_management_system()
-----------------------------------------------------------------------------------------------------------
..Answer 2: Palindrome Checker
This solution checks whether a user-provided string is a palindrome (reads the same forwards and backwards).

Key Features:
Accepts user input string.

Checks if the string is a palindrome (ignores case).

Provides clear feedback to the user.
--------------------------------------------------------
def check_palindrome():
    text = input("Enter a string: ").lower()
    if text == text[::-1]:
        print("Yes, it is a palindrome")
    else:
        print("No, it is not a palindrome")

# Run the function
check_palindrome()
--------------------------------------------------------
..Answer 3: Text Combination and Iteration
This solution combines two user-inputted texts and iterates through each character of the combined string.

Key Features:
Accepts two separate text inputs from the user.

Combines the texts into one string.

Iterates through each character in the combined string and displays them.

----------------------------------------------------------------------
-
def combine_and_iterate_texts():
    text1 = input("Enter first text: ")
    text2 = input("Enter second text: ")
    combined = text1 + text2
    characters = [char for char in combined]
    
    print("Thank you for using my application")
    return characters

# Run the function and print the result
result = combine_and_iterate_texts()
print("Characters in combined text:", result)
--------------------------------------------------------------------------

How to Run the Project:
Ensure Python 3 is installed on your machine.
Copy each solution into a separate .py file or run them individually.
Execute the files using a terminal or any Python-compatible IDE:
------------------------------------------------------------------
python filename.py
------------------------------------------------------------------

Notes:
All the solutions are interactive and require user inputs.
Each solution is independent and can be tested separately.
