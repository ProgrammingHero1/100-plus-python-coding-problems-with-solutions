# 12.2: Password generator

## The Problem

Generate a password. Your password may contain letters in uppercase or lowercase. It also may contain digits or special characters. 

## Hints
To select a random character from a string, you can import random. Then use the random. choice method. This will select a character from the provided string. 

Also, you can import the string module. 

This is not just the string type variable. Instead, it has a lot of extra functionalities.

For example, you can use string.ascii_letters to get all the characters a to z both in lowercase and upper case. Similarly, you can use string.digits to get all the single digits. Also, you can use string.punctuation to get all the special characters.

```python
import string
print('All letters')
print(string.ascii_letters)
print('all digits')
print(string.digits)
print('all special characters')
print(string.punctuation)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Solution
```python
import string
import random
 
def generate_password(size):
   all_chars = string.ascii_letters + string.digits + string.punctuation
   password = ''
   for char in range(size):
       rand_char = random.choice(all_chars)
       password = password + rand_char
   return password
 
pass_len = int(input('How many characters in your password?'))
new_password = generate_password(pass_len)
print('Your new password: ', new_password)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**


## Explanation
The solution is rather simple. We imported the random module and the string module. Then we created a long string by joining all ascii_letters, digits and special characters.

For that, we ran a for loop. In the loop, we select a random letter from the all_chars. To select a random character, we used random.choice. Then we add the random character to the password. 


&nbsp;
[![Next Page](../assets/next-button.png)](Password-with-requirements.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`