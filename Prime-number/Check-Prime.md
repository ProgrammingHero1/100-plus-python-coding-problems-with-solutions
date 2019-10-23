# 7.1 Check Prime: 

##  The problem 
For a given number, check whether the number is a prime number or not.

##   Hint
A number is a prime number. If that number is only divisible by 1 and the number itself. 

This means a prime number is not divisible by any numbers between 1 and the number itself. 

So, to check prime, you can start dividing the number from 2. And then increase it by 1. If the number gets divided, then it’s not a prime number. 

##   The solution 

```python
def is_prime(num):
   for i in range(2,num):
       if (num % i) == 0:
           return False
   return True


num = int(input("Enter a number: "))

check_prime = is_prime(num)

if check_prime:
   print('Your number is a Prime')
else:
   print('Your number is not a Prime')
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

###   Explanation
The core part of the algorithm is the is_prime function. 

There we start a for loop the range(2, num). Because we want to know that the number is not divisible by any number except 1 or the number itself. 

For example, 29. It’s only divisible by 1 or 29. 

So, to test whether the number is divisible by any number greater than 1. We started the for loop from 2. And then going to before the num variable. 

To check the number divisible, we check the remainder to be equal to 0. If the number is gets divided, the remainder will be 0. 

So, if the number gets divided by, it’s not a prime number. That’s why we will return False.

If the number doesn’t get divided by any numbers smaller than the number, it won’t go inside the if block. It will finish all the numbers up to the num. 

Then we will return True. Because it didn’t get divided, by any numbers. Hence, it will be a prime number.

##   Many Solution
There are other solutions to this problem as well. We encourage you to google, “check prime number python”. In that way, you will learn a lot. 

##   Take Away
A prime number is only divisible by 1 and the number itself. 

&nbsp;
[![Next Page](../assets/next-button.png)](Prime-Numbers.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`
