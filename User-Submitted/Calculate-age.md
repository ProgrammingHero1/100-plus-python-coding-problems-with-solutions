# 13.3: Calculate age

## The Problem
Take a birthday of a person and then calculate the age.

This code and solution is contributed by Programmer Karim.

## Hints
Take the user birthday. Use the same method that you used in the previous problem. 

Then, to calculate age, get the days and then divide the days by 365. 

(This is not the perfect way to calculate age...Feel free to find better solutions)

## Solution
This code is contributed by Programmer Karim...

```python
from datetime import datetime
import time
 
 
def calculate_age(born):
	today = datetime.today()
	days = (today-born).days
	age = days // 365
	return age
 
def get_user_birthday():
 date_str = input("Enter your birth date in DD/MM/YYYY: ")
 try:
   birthday = datetime.strptime(date_str, "%d/%m/%Y")
 except TypeError:
   birthday = datetime.datetime(*(time.strptime(date_str, "%d/%m/%Y")[0:6]))
 return birthday
 
birthday = get_user_birthday()
age = calculate_age(birthday)
print("Your age: ", age)
```
 
## Explanation
You used the datetime earlier. And then, calculated the days between the birth date and today’s date. 

Then, divide the days by 365 to get the age!
