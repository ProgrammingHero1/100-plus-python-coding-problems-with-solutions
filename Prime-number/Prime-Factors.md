# Prime Factors

## The problem
Ask the user to enter a number. Then find all the primes factors for the number. 

## Hints
A prime factor is a prime number that could divide a number. 

For example, if you think about the number 35. It has two prime factors: 5 and 7. 

Both 5 and 7 are prime numbers. And they can divide the number 35. 

Similarly, for the number 10, you will have two factors 2 and 5. 

To find the factor, you will run a while loop. 

Before the loop, add an empty list to store the prime number. And a variable named divisor whose starting value is 2.

In the loop, you will start dividing with the number by the divisor. If the number gets divided, add it in the factors list. 

If it is not divided, increase the divisor by 1. 

## The Solution
```python
def get_prime_factors(n):
   factors = []
   divisor = 2
    while n > 2:
       if(n % divisor == 0):
           factors.append(divisor)
           n = n / divisor
       else:
           divisor = divisor + 1
   return factors
 
num = int (input('Enter your number: '))
factors = get_prime_factors(num)
print(factors)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## take Away
Prime factor is a prime number that divides the provided number. 

&nbsp;
[![Next Page](../assets/next-button.png)](Smallest-prime-factor.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`