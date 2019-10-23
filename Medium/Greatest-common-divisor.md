# 9.4 GCD: 

## The Problem
Calculate the greatest common divisor (gcd) of two numbers.

## Hint
In mathematics, the greatest common divisor (gcd) of two or more integers is the largest positive integer that divides each of the integers. 

For example, the gcd of 8 and 12 is 4. Because 4 is the largest number that divides both 8 and 12.

Similarly, 15 is the gcd of 15 and 45. Because 15 divides both 15 and 45.

## The Solution
```python
def compute_gcd(x, y):
	smaller = min(x,y)
	gcd = 1
	for i in range(1, smaller+1):
		if((x % i == 0) and (y % i == 0)):
			gcd = i
	return gcd

num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))

gcd = compute_gcd(num1, num2)

print("GCD of", num1,"and", num2,"is", gcd)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
Since we are trying to find the number that divides both numbers, the dividing number will as big as the smallest number. 

Let’s say you want to get the common divisor of 8 and 24. Their common divisor can not be higher than 8,because the numbers greater than 8 can not divide 8. Hence, the gcd will be smaller or equal to the smallest of the two numbers. 

So, inside the compute_gcd method, we are getting the smallest number by using the min function.

Then, we are running a for loop on the range. The range starts at 1 and goes until the smaller number. 

Inside the loop, we are dividing both numbers by i. If i divides both numbers, we update the gcd, otherwise, we keep going. 

Eventually, we return the gcd. That's it. 

## Recursive GCD
You can use a recursive method to calculate gcd. Just see the solution and know that you can also do it this way.

```python
def gcd(a,b):
    if(b==0):
        return a
    else:
        return gcd(b,a%b)
a=int(input("Enter first number:"))
b=int(input("Enter second number:"))
GCD=gcd(a,b)
print("GCD is: ", GCD)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## built-in GCD
Python has a built-in method to calculate gcd. You can use that one as well. 

```python
import math

a = int(input("Enter first number:"))
b = int(input("Enter second number:"))

gcd = math.gcd(a,b)
print(gcd)
```



&nbsp;
[![Next Page](../assets/next-button.png)](Least-Common-Multiple.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`


