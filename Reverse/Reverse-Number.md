# Reverse a number 

## The problem
Reverse a number. 

## Hints
You have to think differently to reverse a number.

Let’s say you have the number 123. 

`123 = 1 * 100 + 2 * 10 + 3`

First, you have to take the last digit of the number. You have done this many times. Just divide the number by 10 and get the remainder. 

Once you have the last digit. Add it to a variable named reverse. 

And get rid of the last digit by performing a floor division by 10.  Then your 123//10 will make the remaining number 12. 

In the next step, get the last digit of the remaining number (12) which will be 2. Multiply the reverse number by 10 and then add the new last digit. That's why your new reverse number will become 30+2. This will be 32. 

Once again perform a division on the remaining number. 12//10 will make it 1. 

In the last step, multiply the reverse number by 10. It will become 320 and add the remainder 1. The total number will become 320 + 1 = 321.

This is the overall process to reverse a number. 

Now, think about the overall algorithm.

## Solution
 
```python
def reverse_num(num):
   reverse = 0
   while(num>0):
       last_digit = num%10
       reverse = reverse*10 + last_digit
       num = num//10
   return reverse
 
n=int(input("Enter number: "))
reverse = reverse_num(n)
print("Reverse of the number:",reverse)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
Once you understand the hint, the algorithm will become super easy. 

Inside the while loop, we are getting the last digit by getting remainder. Then we set the new reverse number by multiplying the previous reverse number by 10 and then we are adding the last digit.

Finally, set the new value of the num by dividing by 10. 

That’s it. 

&nbsp;
[![Next Page](../assets/next-button.png)](Reverse-word.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`

