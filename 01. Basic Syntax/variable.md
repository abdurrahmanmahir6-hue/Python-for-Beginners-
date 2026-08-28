# Variable
A variable in Python is a box that stores data or values.

## What a variable does
1. storing data such as numbers, text list
2. It is easy to change the value.
3. Variables can be used many times within a program.


## Understand with real life analogy
> "Imagine you have a number of empty boxes. You use a marker to write 'Age' on one box and 'Name' on another.Next, you place the number 15 inside the box marked 'Age'. After some time, once your birthday has passed, you remove the 15 from the box, discard it, and replace it with 16. Yet, the 'Age' label on the box stays precisely as it was.In programming, a variable functions exactly like this labeled box.”

## Code example 
```python
# Example 1: Creating a simple variable (putting an item in a box) 

student_name = "Rahim"       	# "Rahim" is placed in the box named 'student_name' 
student_age = 15      			# 15 is placed in the box named 'student_age' 
print("Student's name:", student_name) 
print("Student's age:", student_age)     

# Example 2: Changing a variable's value (the real magic of variables!) 
student_age = 16 					# The previous value (15) is removed and replaced with 16 
print("Age after one year:", student_age) 

# Example 3: Performing simple math using variables 
math_marks = 80 
english_marks = 70 				# The values from the two boxes are added together and stored in a new box named 'total_marks' 
total_marks = math_marks + english_marks 
print("Total marks:", total_marks)

# Example 4: Assign and change value at the same time
value = 10
value += 5
print(value) 	# output is 15
print(value -= 7) 	# output is 8
```
> Note: "+=", "-=", "*=" These are called assignment operators. We will learn about them in the operator topic.

## 6 Golden Rules for Writing Variables in Python
1. Names should never start with a number ❌
   Variable names should always start with a letter (a-z, A-Z) or an underscore (_).
```python
✅ Correct: student1, age_20, _marks
❌ Incorrect: 1student, 20age, 1st_player
```

2. Variable names cannot contain spaces ❌
   Use underscores _ to separate multiple words.
```python
✅ Correct: student_name, total_marks, my_age
❌ Incorrect: student name, total marks, my age
```

3. Special characters or Symbols cannot be used ❌
   Using symbols like @, #, $, %, !, -, *, +, / etc. in the name is strictly prohibited. Only underscores (_) can be used.
```python
✅ Correct: student_name, score100
❌ Incorrect: student@name, score-100, price$
```

4. Do not use Python's Reserved Keywords ❌
   Python has built-in keywords reserved for specific functions. You cannot use these as variable names
```python
❌ Keywords: if, else, for, while, class, def, return, True, False, None, import
```

5. Case-Sensitive (Distinguishing uppercase and lowercase letters) ⚠️Computers treat uppercase and lowercase letters as completely different. Therefore, Age, age, and AGE are three distinct variables.
```python
age = 10
Age = 15
print(age)  # output is  10
print(Age)  # output is 15
```

6. Use meaningful and short names ✅ (Best Practice)
The variable name should be clear enough so that reading the code explains what data it holds. Single-letter names (a, b, x, y) should be avoided (except in mathematical formulas).
