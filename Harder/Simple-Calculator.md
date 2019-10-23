# 12.1 Simple Calculator

## The task
Create a simple calculator. That will be able to take user input of two numbers and the operation the user wants to perform.

## Solution strategy
Create a bunch of functions to perform add, subtract, multiply, division or modulo. 

Then take two numbers from the user and the operation he/she wants to perform. Either +,-,*,/ or %.

Then call the appropriate function based on the operation.

Think for a few minutes and try it yourself first.

## The solution
```python
def add(num1, num2):
 return num1 + num2
 
def subtract(num1, num2):
 return num1 - num2
 
def multiply(num1, num2):
 return num1 * num2
 
def divide(num1, num2):
 return num1 / num2
 
def modulo(num1, num2):
 return num1 % num2
 
# Take input from the user
num1 = int(input("Enter first number: "))
operation = input("What you want to do(+, -, *, /, %):")
num2 = int(input("Enter second number: "))
 
result = 0
if operation == '+':
 result = add(num1,num2)
elif operation == '-':
 result = subtract(num1,num2)
elif operation == '*':
 result = multiply(num1,num2)
elif operation == '/':
 result = divide(num1,num2)
elif operation == '%':
 result = modulo(num1,num2)
else:
 print("Please enter: +, -, *, / or %")
 
print(num1, operation, num2, '=', result)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**


## How it works
You saw five functions to add, subtracts, etc. Those are easy.

Then we are taking user inputs. Three inputs. They are easy too. 

Then we have if-elif-else. And based on the operation, we call the right method to perform the task.

That’s it. 


&nbsp;
[![Next Page](../assets/next-button.png)](Password-generator.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`