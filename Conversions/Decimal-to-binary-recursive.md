# 4.4: Decimal to Binary (recursive) 

## The Problem
Convert a decimal number to binary number using a recursive function. 
###  Hints 
After coding for a while, recursive will become fun. Until then, recursive functions might feel like confusing magic. 

So, don’t worry if you felt confused. You are not alone. I am in the same condition as well.

## Recursive
```python
def dec_to_binary(n):
   if n > 1:
       dec_to_binary(n//2)
   print(n % 2,end = '')
```

## decimal number
```python
num = int(input("Your decimal number: "))
dec_to_binary(num)
print(" ")
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
The core part of the logic is simple. If the number is greater than 1, call the dec_to_binary function again. And, while calling, send the result of dividing operation as the input number. 

If you remember, the while loop in the previous code problem is similar. In the while loop, we were going back to the next iteration with n = n//2

Here we are calling the same function with the n//2

In the previous code problem (iterative), we are putting the remainder in a list. Here, we are printing it right away. 

While printing, we have one extra thing called end=''. 
The purpose of end='' is to print the output in the same line. If you don’t add end='', every print output will be displayed in a new line. 


## Take Away
There are multiple ways to format the print string. Google it, when needed.


&nbsp;
[![Next Page](../assets/next-button.png)](../Solution-Strategy.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`
