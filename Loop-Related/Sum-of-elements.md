# 3.1: Sum of elements

## The Problem
For a given list, get the sum of each number in the list

## Hint
Should be simple for you. Declare a sum variable. Then just loop through the list and add it to the sum. 

## The solution
```python
def get_sum(nums):
   sum = 0
   for num in nums:
       sum = sum + num
   return sum
 
 
nums = [13,89,65,42,12,11,56]
 
total = get_sum(nums)
print("The total of each elements:",total)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation: 
It’s super simple. 

You got a list. Loop through the list. You have done that multiple times while learning Fundamentals. 

Declare a variable named sum before the loop. And inside the loop, add the number to the sum variable. 

And then finally return the sum.

That’s it. 
Super easy. Even your grandma can do it.

## Shortcut

There is an easier way to get sum of all numbers in a list. You can just pass the list of numbers to the sum function.
```python
nums = [13, 11, 16, 78, 31, 128]

total = sum(nums)
print(total)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Quiz

What is the shortcut way to sum all the numbers in a list?

1. Loop through the items
2. Use the sum function
3. Use a calculator

<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is: 2</p>
 </details>

## Take Away

Use the sum function to sum all the numbers in a list.


&nbsp;
[![Next Page](../assets/next-button.png)](Largest-element-of-a-list.md)
&nbsp;