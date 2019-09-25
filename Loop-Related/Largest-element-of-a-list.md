
## 3.2 Largest element of a list

#### S-1: The problem
Find the largest element of a list.

<details>
 <summary><b>S-2: Click Here For Show Hints</b></summary>
   <p>Take the first element as the largest number. Then loop through the list and compare each element.
 </details>
<br>

#### S-3: Solution
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
**[Try It:](/https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

#### S-4: Explanation
In the beginning, consider the first element of the list as the largest element. 

Don’t set the largest value to 0. If every number in the list is a negative number, your return will be wrong. 

Then just loop through the list and compare. If the current number is greater than the largest number, set it as the largest number. 

That’s it. Easy peasy. 

#### S-5: Shortcut
One shortcut is to  pass a list of numbers to the max function. This will return the largest number in the list.

```python
nums = [41, 69, 23, 45, 19, 8]

largest = max(nums)
print(largest)
```
**[Try It:](/https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

#### S-6: Quiz
What is the easiest way to find the largest number in a list?
1. Use the max function
2. Use the min function
3. Use the sum function

#### S-7: Take Away

Use the max function to get the largest number in a list.

&nbsp;
[![Next Page](../assets/next-button.png)](Sum-of-squares.md)
&nbsp;

###### tags: `programmig-hero` `python` `float` `int` `math`

