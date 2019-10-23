
# Second Largest

## The problem
For a list, find the second largest number in the list.

## Hints
Finding the largest number was super easy. To find the second largest number, you have to keep track of two variables. Then compare.

## Solution
```python
def get_second_largest(nums):
   largest = nums[0]
   second_largest = nums[0]
   for i in range(1,len(nums)):
       if nums[i] > largest:
           second_largest = largest
           largest = nums[i]
       elif nums[i] > second_largest:
           second_largest = nums[i]
   return second_largest
 
my_nums = [44,11,83,29,25,76,88]
second_largest = get_second_largest(my_nums)
print("Second highest number is : ",second_largest)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
We declared two variables. One is called the largest. Another one is second_largest. We started both with the value of the first element of the list. 

Then we ran a for loop on range. The range looks like range(1, len(nums)). We started the list with 1 because we already set the first value as the largest and second_largest. Then the upper value of the range is len(nums). 

This means the range should run up to the length of the list. 

Inside the loop, we have an if-else block. If the current element num[ i ] greater than the current largest element. This means the current largest element will become the new second largest element. And the current element will become the largest element. 

On the other hand, if the current value is greater than the current second largest element, we just set the current value as the second largest element. 

That's it.

## Think Different
Can you think about any way to solve this problem?

One clever solution could be, 

Step 1: Use the max function to find the largest number. 
Step 2: Remove the max number from the list
Step 3: From the remaining numbers, find the max number. As you already remove the previous max number, this max number will be the second-largest number.

How cool is this solution?

## Clever Solution

```python
nums = [5, 12, 54, 87, 55, 69, 23, 17]
nums.remove(max(nums))
second_largest = max(nums)
print(second_largest)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**


## Take Away
Clever ways to solve problems will make you happier.

&nbsp;
[![Next Page](../assets/next-button.png)](Second-smallest.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`

