
## 2.1 max of two

#### S-1: The problem
Find the max number of two numbers.

<details>
 <summary><b>S-2: Click Here For Show Hints</b></summary>
   <p> Ask the user to enter two numbers. 

Then, you can run a comparison to compare which one is larger. 

Think about it and try yourself first. 
 </p>
 </details>
<br>

#### S-3: Solution
```python
num1 = int(input("First number: "))
num2 = int(input("Second number: "))
if (num2 >= num1):
    largest = num2
else:
    largest = num1
print("Largest number you entered is: ", largest)
```
**[Try It:](/https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

#### S-4: Shortcut
Another simple and alternative solution is to send the numbers to the max function.
```python
num1 = int(input("First number: "))
num2 = int(input("Second number: "))
largest = max(num1, num2)
print("Largest number you entered is: ", largest)
```
**[Try It:](/https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

#### S-5: Alternative Solution
Another alternative approach is to use the floor method from the math module. If you pass a number with a fraction to the math.floor function, it will return you the integer part of the number. 

For example, 
```python
import math
result = math.floor(3.4)
print(result)
```
**[Try It:](/https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

#### S-6: Alternative Solution
Do you want to see your name in this app as a contributor?

If yes, find a better solution or alternative solution of any of the problems here. Then, send your solution with a code explanation to programming.hero1@gmail.com

If your solution is approved by the Team Programming Hero, we will publish your solution in the app with your name as the contributor. 

> That would be fun.

&nbsp;
[![Next Page](../assets/next-button.png)](Max-of-three.md)
&nbsp;

###### tags: `programmig-hero` `python` `float` `int` `math`

