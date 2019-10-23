
# Largest element of a list

## The problem
Find the largest element of a list.

## Hints
Take the first element as the largest number. Then loop through the list and compare each element.
 

## Solution
```python
def get_largest(nums):
   largest = nums[0]
   for num in nums:
       if num > largest:
           largest = num
   return largest
 
my_nums = [0,15,68,1,0,-55]
 
largest = get_largest(my_nums)
 
print('The largest number is: ', largest)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
In the beginning, consider the first element of the list as the largest element. 

Don’t set the largest value to 0. If every number in the list is a negative number, your return will be wrong. 

Then just loop through the list and compare. If the current number is greater than the largest number, set it as the largest number. 

That’s it. Easy peasy. 

## Shortcut
One shortcut is to  pass a list of numbers to the max function. This will return the largest number in the list.

```python
nums = [41, 69, 23, 45, 19, 8]

largest = max(nums)
print(largest)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Quiz
What is the easiest way to find the largest number in a list?
1. Use the max function
2. Use the min function
3. Use the sum function


## Take Away

Use the max function to get the largest number in a list.

&nbsp;
[![Next Page](../assets/next-button.png)](Sum-of-squares.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`

