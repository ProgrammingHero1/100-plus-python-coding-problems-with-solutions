# 12.3: Password with Requirements [Premium]

## The Problem
Generate a password that has a minimum of one uppercase, one lowercase, one digit, and one special character

## Hint
This one is easier. The string module has two more things to get the uppercase and lower case characters...

```python
import string
print('All letters')
print(string.ascii_letters)
print('Al lowercase characters')
print(string.ascii_lowercase)
print('All uppercase characters')
print(string.ascii_uppercase)
```
 
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Solution
```python
import random
import string
 
def randomPassword(size):
	all_chars = string.ascii_letters + string.digits + string.punctuation
	password = ""
	password += random.choice(string.ascii_lowercase)
	password += random.choice(string.ascii_uppercase)
	password += random.choice(string.digits)
	password += random.choice(string.punctuation)
	
	for i in range(size-4):
		password += random.choice(all_chars)
	return password
 
pass_len = int(input("What would be the password length? "))
print ("First Random Password is:", randomPassword(pass_len))
print ("Second Random Password is:", randomPassword(pass_len))
print ("Third Random Password is:", randomPassword(pass_len))
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
The all_chars variable is the same as before. After that, we created a password variable with an empty string. 

Then, we added random choice from lowercase. This way, we will make sure that at least one lowercase character is added in the password. Similarly, we added one uppercase, one digit, and one special character.

After that, we ran a for loop to select random characters from the all_chars. This is similar to the previous problem. We just ran the for loop for (size-4) times, because we already added 4 characters in the password before the loop.

Make sense?

Keep going. Only a few more left. I am sure you can do it 


&nbsp;
[![Next Page](../assets/next-button.png)](Permutations.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`