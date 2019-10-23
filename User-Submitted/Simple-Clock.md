# 13.1 Simple Digital Clock

## The Task
Create a simple clock.

This problem and code example is created by Steine Chaos / Malte Lupin.

If you want to see your name as a contributor to the app, find a code example that we don’t have here, and email it at programming.hero1@gmail.com

## Solution Strategy
Two things would be new for you here. 

Let’s talk about the global keyword first. 

Inside a function, you can use two types of variables: any variable declared inside the function or the parameter. 

If you want to set or update the value of any variable declared outside of the function, you can either pass it as a parameter. In that case, it will not update the value of the variable outside of the function. In the code below, you will have the value of x remained as 5. 

```python
x = 5
 
def double_global_x(x):
 x = 2*x
 return x
 
print('use global keyword')
result = double_global_x(x)
print(result)
print('Updated value of x:', x)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

If you want to change the value of the variable inside a function, you have to use the global keyword. Just add a new line and put global and then the name of the variable. In that case, python will know that it will read and set value from the variable outside of the function. For example, in the code below the value of the x will become 10. 

```python
x = 5
 
def double_global_x():
 global x
 x = 2*x
 return x
 
print('use global keyword')
double_global_x()
print(result)
print('Updated value of x:', x)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Time module
There is a built-in module in python named time. It has a lot of time-related functionalities. One function on the time module is called sleep. The sleep takes a parameter named sec. 

You can pause your function wait for a certain number of sec and then execute it. 

For example, we can run an infinite loop and after every second you can print Tick

```python
import time
 
while True:
 time.sleep(1)
 print('Tick')
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## The solution
This code is submitted by: Steine Chaos / Malte Lupin
 
```python
import time
 
print('Simple clock made by Steine Chaos:\n')
 
hour = int(input("Type in the current hour:"))
minute = int(input("Type in the current minute:"))
second = int(input("Type in the current second:"))
 
def display():
	print(hour, ':', minute, ':', second)
 
def add():
	global hour
	global minute
	global second
	
	second=second+1
	if second==60:
		minute=minute+1 
		second=0
	if minute==60:
		hour=hour+1 
		minute=0
	if hour==24:
		hour=0
 
print('\n')
 
while True:
	time.sleep(1)
	add()
	display()
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## How it works
The code is simple...We imported the time module, then, asked the user for three inputs: for the current hour, minute, and second. 

Then, we have two methods: One to display hour, minute and second. Another, to add a second. We will look at the add method a little later. First, look at the bottom part. 

We have an infinite loop, because we don’t want the clock to stop. We want the clock to run forever until we stop it. 

And, inside the loop, we call the display and the add method and then, we call the time.sleep and pass 1. 

By default, the while loop runs immediately. However, inside the while loop, the first thing we have is the time.sleep(1). This is telling the loop to wait for 1 second. Then we are calling the add function. When add is done, we are calling the display function to display the hour, minute, and seconds. 

The add function is a bit interesting...

We are accessing three global variables: hour, minute, and second, and we are increasing the second by 1. 

This is the main task. However, if the second becomes 60, we increase a minute and set second to 0, because 60 seconds are equal to a minute. 

Similarly, if the minute becomes 60, we add 1 hour and set minutes to 0, because 60 minutes is 1 hour. 

Finally, if the hour is 24, we reset the hour to 0. Because, in a digital clock, there are no 24 or 25 hours. After 23 hours, it becomes 0 hours again (the midnight!) 


&nbsp;
[![Next Page](../assets/next-button.png)](Birthday-remaining.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`