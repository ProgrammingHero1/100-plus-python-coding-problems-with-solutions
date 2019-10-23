
# max of three

## The problem
Find the largest of the three numbers.

## Hints
Ask the user to enter three numbers. 

Then, you can run multiple comparisons to compare which one is the largest. 

At first, you can consider that the first number is the largest. 

Then compare the second number with the first number and the third number. If the second number is greater or equal to the first number and the second number is greater or equal to the third number, then the second number is the largest. 

Similarly, compare the third number with the first or second number. 

Otherwise, the first number will be the largest. 

Think about it. And try yourself first.

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Solution
```python
num1 = int(input("First number: "))
num2 = int(input("Second number: "))
num3 = int(input("Third number: "))
 
largest = num1
 
if (num2 >= num1) and (num2 >= num3):
   largest = num2
elif (num3 >= num1) and (num3 >= num2):
   largest = num3
else:
   largest = num1
 
print("Largest number you entered is: ",largest)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

####   Shortcut
Another simple and alternative solution is to send the numbers to the max function. 
```python
num1 = int(input("First number: "))
num2 = int(input("Second number: "))
num3 = int(input("Third number: "))
 
largest = max(num1, num2, num3)
 
print("Largest number you entered is: ",largest)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Quiz
What is the easiest way to find out the largest number?

1. Use multiple if-else conditions
2. Use the max function
3. All numbers are created equal

<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is : 2</p>
 </details>

## Take Away
Use the max function to get the largest number.

&nbsp;
[![Next Page](../assets/next-button.png)](Average-of-numbers.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving` 