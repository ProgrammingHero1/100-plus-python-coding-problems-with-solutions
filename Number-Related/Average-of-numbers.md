
# Average of numbers

## The problem
Take numbers from a user and show the average of the numbers the user entered. 

## Hints
To solve this problem. 
 
First, ask the user - How many numbers you want to enter?

Then, run a for-loop. Each time, take input from the user and put it in a list. 

Once you get all the numbers, you can send the list to the sum function. The sum function will add all the numbers and give you the total. 

Finally, divide the total by the number of elements the user entered. 

That’s it, you will get the answer. 

Want to try it yourself first? Go to the code editor and try it.

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**


## Solution
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

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
First, ask the user how many numbers he/she wants to enter. Once we have the number, run a for loop. To collect the numbers. 

While collecting the numbers, we are adding those in the list called nums.

Then we pass the list to the sum function. The sum function returns us the sum of each number in the list

Eventually, we divide the total by the number of elements to get the average.

## Another Solution
```python
len=int(input("How many numbers you want to enter: "))
 
total = 0
 
for i in range(0,len):
   elem=int(input("Enter element: "))
   total += elem
 
avg = total/len
print("Average of elements you entered",round(avg,2))
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
In the second approach, other than directly adding to the list, we are adding it to the total variable. And then we are dividing it by the number of input the user entered. 

## Take Away
> To get the average, calculate the total and divide by the number of elements.

&nbsp;
[![Next Page](../assets/next-button.png)](Divisible-by-3-and-5.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving` 