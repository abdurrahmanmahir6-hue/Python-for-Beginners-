# Variable
A variable in Python is a box that stores data or values.

## What a variable does
1. storing data such as numbers, text list
2. It is easy to change the value.
3. Variables can be used many times within a program.


## Understand with real life analogy
"Imagine you have a number of empty boxes. You use a marker to write 'Age' on one box and 'Name' on another.Next, you place the number 15 inside the box marked 'Age'. After some time, once your birthday has passed, you remove the 15 from the box, discard it, and replace it with 16. Yet, the 'Age' label on the box stays precisely as it was.In programming, a variable functions exactly like this labeled box.”

Code ex
# Example 1: Creating a simple variable (putting an item in a box) 

student_name = "Rahim"       # "Rahim" is placed in the box named 'student_name' 
student_age = 15      # 15 is placed in the box named 'student_age' 
print("Student's name:", student_name) 
print("Student's age:", student_age)     # 

Example 2: Changing a variable's value (the real magic of variables!) student_age = 16 # The previous value (15) is removed and replaced with 16 print("Age after one year:", student_age) # Example 3: Performing simple math using variables math_marks = 80 english_marks = 70 # The values from the two boxes are added together and stored in a new box named 'total_marks' total_marks = math_marks + english_marks print("Total marks:", total_marks)
