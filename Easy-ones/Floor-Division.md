
# Floor division

## The problem
Find the floor division of two numbers. 

## Hints
Floor division means the integer part of a division operation. For example, if you divide 17/5 the quotient will be 3.4.

**Here the integer part is 3.**

> So, you have to find the integer part of the division operation.

## Solution

```python
num1 = int(input('Enter the first number: '))
num2 = int(input('Enter the second number: '))
 
result = num1//num2
print(result)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
When you divide one number by another you get two things. One is called the integer part of the division. Another is the remainder. 

To get the quotient (result without the remainder), you can use two-division symbols. 
```python
print(37//10)
37 = 3*10+7
```

## Think different
Another alternative approach is to use the floor method from the math module. If you pass a number with a fraction to the math.floor function, it will return you the integer part of the number. 

For example, 
```python
import math
result = math.floor(3.4)
print(result)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

####   Alternative Solution
Now, you can use the floor function to get the floor the division. Like below-
```python
import math
num1 = int(input('Enter the first number: '))
num2 = int(input('Enter the second number: '))
 
result = math.floor(num1/num2)
print(result)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Quiz
How will you get a floor division?

1. //
2. /
3. %
  
<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is : 1</p>
 </details>

## Take Away
Use // to get floor division.

&nbsp;
[![Next Page](../assets/next-button.png)](Temporary-variable.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`

