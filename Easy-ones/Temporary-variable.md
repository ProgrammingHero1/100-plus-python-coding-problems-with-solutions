
## 1.5: Swap two variables

**S-1: The problem**
> Swap two variables.<br><br>To swap two variables: the value of the first variable will become the value of the second variable. On the other hand, the value of the second variable will become the value of the first variable. 

<details>
   <summary><b>S-2: Click Here For Show Hints</b></summary>
   <p>To swap two variables, you can use a temp variable.</p>
 </details>
<br>

#### S-3: Solution

```python
a = 5
b = 7
print('a, b', a, b)
# swap these two
temp = a
a = b
b = temp
print('a, b', a, b)
```
**[Try It:](/https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## S-4: Shortcut
You can use a python shortcut to swap two variables as well. How this works, would be a little bit tricky for you. So, for now, just remember it.

```python
x = 12
y = 33
print('x, y', x, y)
#swap these two
x, y = y, x
print('x, y', x, y)
```
**[Try It:](/https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

#### S-5: Another solution
If both the variable is number, you can apply other tricks. Like the one below-

```python
a = 5
b = 7
print('a, b', a, b)
# swap these two
a = a + b
b = a - b
a = a - b
print('a, b', a, b)
```
**[Try It:](/https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

#### S-6: Quiz
How would you swap two variables?

1. Using two temporary variables
2. My family doesn’t permit swapping
3. Use something like: a, b= b, a

**The answer is: 3**

*S-7: Take Away*
Use temp variable to swap two variables. <br>

&nbsp;
[![Next Page](../assets/next-button.png)](#)
&nbsp;

###### tags: `programmig-hero` `python` `float` `int` `math`


