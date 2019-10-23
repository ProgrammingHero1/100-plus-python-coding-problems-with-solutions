
# Second smallest element

## The problem
For a list, find the second smallest element in the list

## Hints 
If you understand the process of finding the second largest element, this will be a piece of cake for you.

## Solution
```python
def get_second_smallest(nums):
   smallest = nums[0]
   second_smallest = nums[0]
   for i in range(1,len(nums)):
       if nums[i] < smallest:
           second_smallest = smallest
           smallest = nums[i]
       elif nums[i] < second_smallest:
           second_smallest = nums[i]
   return second_smallest
 
my_nums = [44,11,83,29,25,76,88]
second_smallest = get_second_smallest(my_nums)
print("Second smallest number is : ", second_smallest)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
We declared two variables. One is called the smallest. Another one is second_smallest. We started both with the value of the first element of the list. 

Then we ran a for loop on the range. The range looks like range(1, len(nums)). We started the list with 1 because we already set the first value as the smallest and the second smallest. Then the upper value of the range is len(num). 

This means the range should run up to the length of the list. 

Inside the loop, we have an if-else block. If the current element num[ i ] smaller than the current smallest element. This means the current smallest element will become the new second smallest element. And the current element will become the smallest element. 

On the other hand, if the current value is smaller than the current second smallest element, we just set the current value as the second smallest element. 

That's it.

## Think DIfferent

You can use the previous clever solution to find the second smallest number as well. 

Please note that, by removing an element from the list, you are changing the original list. If you don’t want to modify the list (you might need the list for other operations), you should use the comparison method. 

## Clever Solution

```python
nums = [2, 15, 14, 71, 52, 209, 551]
nums.remove(min(nums))
second_smallest = min(nums)
print(second_smallest)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Take Away
If you know multiple solutions to a problem, you can apply the right solution based on the situation.

&nbsp;
[![Next Page](../assets/next-button.png)](Remove-duplicate-Chars.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`

