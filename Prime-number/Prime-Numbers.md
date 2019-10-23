# 7.2 All Prime Numbers

## the problem
Ask the user to enter a number. Then find all the primes up to that number. 

## Hints

You can use the previous is_prime function that you created in the previous problem. Now create a new function named all_primes. In that function, run a for loop. 

For each number, call the is_prime function. If the return is True to add it in the prime list. 

## The Solution
```python
 def is_prime(num):
  for i in range(2,num):
      if (num % i) == 0:
          return False
  return True
 
def all_primes(num):
  primes = []
  for n in range(2,num+1):
      if is_prime(n) is True:
          primes.append(n)
  return primes
 
num = int(input("Enter upper limit: "))
primes = all_primes(num)
print(primes)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
The first one is the is_prime that you have seen before. Now we created another function named all_primes. In the all_primes function, we create a list named primes to hold the prime numbers. Then run a for loop using range.

The range starts at 2 and runs until num+1 so that it goes until num. We are starting at 2. Because 2 is the first prime number. 

Inside the loop, call the is_prime function and check the return. If the return is True then append the n in the primes list. 

Then return the primes list. 

That’s it.

&nbsp;
[![Next Page](../assets/next-button.png)](Prime-Factors.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`