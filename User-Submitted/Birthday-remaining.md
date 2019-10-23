# 13.2 Birthday remaining

## The problem
Calculate how many days are remaining for the next birthday.

This code is submitted by Programmer Karim.

## Hints
Let’s say, you want to display 5 random numbers. You can write the code like below:

```python
import random
print(random.randint(0,10))
print(random.randint(10,20))
print(random.randint(20,30))
print(random.randint(30,40))
print(random.randint(40,50))
```
 
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**


The problem is that, in every line, you have to type random.randint. As a programmer, you will be lazy. Hence, while import you can import the randint directly in your code. For that, you have to say, from random import randint. Like below:

```python
from random import randint
print(randint(0,10))
print(randint(10,20))
print(randint(20,30))
print(randint(30,40))
print(randint(40,50))
```
 
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Solution
The code below is submitted by Programmer Karim...

```python
from datetime import datetime
import time
 
def get_user_birthday():
 date_str = input("Enter your birth date in DD/MM/YYYY: ")
 try:
   birthday = datetime.strptime(date_str, "%d/%m/%Y")
 except TypeError:
   birthday = datetime.datetime(*(time.strptime(date_str, "%d/%m/%Y")[0:6]))
 return birthday
 
def days_remaining(birth_date):
  now = datetime.now()
  current_year = datetime(now.year, birth_date.month, birth_date.day)
  days = (current_year - now).days
  if days < 0:
    next_year = datetime(now.year+1, birth_date.month, birth_date.day)
    days = (next_year - now).days
  return days
 
birthday = get_user_birthday()
next_birthday = days_remaining(birthday)
print("Your birthday is coming in: ", next_birthday, " days")
```

## Explanation
We imported the datetime method from the datetime module. It has a lot of good functionalities.

First, in the get_user_birthday function, we take user birthday in a format of DD/MM/YYYY. This means we are telling the user to insert the date of his/her birthday first then a forward slash followed by the month and year in four-digits. 

Then, we convert the birthday in a python date by using datetime.strptime function. To that function, we have to pass the date in the string and the format of the date. The format of the date is %d/%m/%Y. 


We also imported time. Sometimes, strptime gives some Type exception. For that reason, we put a  try-except there.


If you convert a date string to a python date, then you can easily access the day, month and year and do some extra calculation over the date. 

We have another method called days_remaining. In that method, we first get the date of now. This is actually the date of the time right now. It is the time when you run the code.

Then, you calculate the users' birthday of the current year. It’s simple...you just take the year from now (current year) with month and date from users' birthday. 

The next thing is very simple...you just get the difference between the user’s birthday in the current year and now, and ultimately get the days. 

If the birthday for this year is over, the difference will be negative, because the birthday for this year has already passed. Then, we get the birthday for the next year by adding one(1) with the current year and with the month and the day from the birth date. 

At last, we calculate the difference. 

That’s a pretty simple way to get the days remaining for your next birthday.

Isn’t it cool? 


&nbsp;
[![Next Page](../assets/next-button.png)](Calculate-age.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`