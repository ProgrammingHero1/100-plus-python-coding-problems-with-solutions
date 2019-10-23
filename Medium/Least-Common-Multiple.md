# 9.5: LCM

## The Problem
For two numbers, calculate the least common multiple (LCM).

## Hint
The multiples of 4 and 5 are below:

Multiple of `4: 4,  8,  12, 16, 20 , 24 28 ,32, 36, 40, 44`
Multiple of `5: 5, 10, 15, 20, 25, 30, 35, 40, 45, 50, 55 `

Now, what are the common multiples? The common number that exists in multiple of 4 and 5 are:

Common multiples: `20, 40, 60, 80`

So, you can tell the smallest common multiple is 20. Hence, the least common multiple(LCM) of 4 and 5 is 20.

## The solution
```python
def calculate_lcm(x, y):
	lcm = max(x,y)
	while lcm % x != 0 or lcm % y != 0:
		lcm += 1
	return lcm
 
num1 = int(input("First number: "))
num2 = int(input("Second number: "))
lcm = calculate_lcm(num1, num2)
 
print(f"LCM of {num1} and {num2} is: {lcm}")
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
First, we calculate the greater number, because LCM will be equal or higher than the highest of the two numbers. 

Another important point is: we know where the loop will start. It will be the highest of the two numbers. However, we don’t know where it will stop. That’s why we can’t use a for loop with a range. 

Instead, we used a while loop. 

In the while loop, if we can not divide the lcm by the first number or the second number, we keep increasing the lcm. 

That's it. 

It's actually much easier than it seems. 



&nbsp;
[![Next Page](../assets/next-button.png)](../Programming-Contest/Programming-Contest.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`

