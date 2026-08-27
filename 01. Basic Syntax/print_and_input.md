# Print and Input
## print()
print means to display a specific object on the console.

The print function is used to display something in python.
> print()

If I tell python to display “Hello, World!” then we have to call the print() function.
```python
print(“Hello, World!”)
```
Output:
```text
Hello, World!
```

To print any text, we have to give a double quite or a single quite. If we do not give quite, python will not understand that Hello, World! is a text, it has to be printed.

We do not have to use quite to print a number. We can write the number directly.
```python
print(10)
print(5.6)
print(10+10)
```
Output:
```text
10
5.6
20
```
> note: if we write something between quite, python sees it as text.

## input()

In Python, the input() function is used to get data from the user.
For example, if I want to get the user's name input, the python syntax will be:
```python
name = input(“Enter your name: ”)
```
The input() function always takes text data type. If we want to get a number as input, we have to do type casting.
