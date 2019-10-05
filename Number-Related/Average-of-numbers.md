
## 2.3: Average of numbers

#### S-1: The problem
Take numbers from a user and show the average of the numbers the user entered. 

<details>
 <summary><b>S-2: Click Here For Show Hints</b></summary>
   <p>To solve this problem. 
 
First, ask the user - How many numbers you want to enter?

Then, run a for-loop. Each time, take input from the user and put it in a list. 

Once you get all the numbers, you can send the list to the sum function. The sum function will add all the numbers and give you the total. 

Finally, divide the total by the number of elements the user entered. 

That’s it, you will get the answer. 

Want to try it yourself first? Go to the code editor and try it.
</p>
 </details>
<br>

**[Try It:](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**


#### S-3: Solution
```python
len = int(input("How many numbers do you want to enter? "))
 
nums = []
 
for i in range(0, len):
   element = int(input("Enter element: "))
   nums.append(element)
 
total = sum(nums)
avg = total/len
print("Average of elements you entered",round(avg,2))
```

**[Try It:](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

#### S-4: Explanation
First, ask the user how many numbers he/she wants to enter. Once we have the number, run a for loop. To collect the numbers. 

While collecting the numbers, we are adding those in the list called nums.

Then we pass the list to the sum function. The sum function returns us the sum of each number in the list

Eventually, we divide the total by the number of elements to get the average.

#### S-5: Another Solution
```python
len=int(input("How many numbers you want to enter: "))
 
total = 0
 
for i in range(0,len):
   elem=int(input("Enter element: "))
   total += elem
 
avg = total/len
print("Average of elements you entered",round(avg,2))
```
**[Try It:](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

#### S-6: Explanation
In the second approach, other than directly adding to the list, we are adding it to the total variable. And then we are dividing it by the number of input the user entered. 

#### S-7: Take Away
> To get the average, calculate the total and divide by the number of elements.

&nbsp;
[![Next Page](../assets/next-button.png)](Divisible-by-3-and-5.md)
&nbsp;

###### tags: `programmig-hero` `python` `float` `int` `math` 