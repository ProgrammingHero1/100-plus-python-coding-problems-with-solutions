
# Swap two variables

## The problem
> Swap two variables.<br><br>To swap two variables: the value of the first variable will become the value of the second variable. On the other hand, the value of the second variable will become the value of the first variable. 

## Hints
   To swap two variables, you can use a temp variable.

## Solution

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
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Shortcut
You can use a python shortcut to swap two variables as well. How this works, would be a little bit tricky for you. So, for now, just remember it.

```python
x = 12
y = 33
print('x, y', x, y)
#swap these two
x, y = y, x
print('x, y', x, y)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Another solution
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
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Quiz
How would you swap two variables?

1. Using two temporary variables
2. My family doesn’t permit swapping
3. Use something like: a, b= b, a

<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is : 3</p>
 </details>

## Take Away
Use temp variable to swap two variables. <br>

&nbsp;
[![Next Page](../assets/next-button.png)](../Number-Related/max-of-two.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`


