# 11.4: Bulls and Cows (4 digits) 

## The Problem

Create a bulls and cows game for guessing a randomly generated 4 digits number. 

## Hints
This one should be easier for you. Just make sure that the random number is four digits. Hence, it should be between 1000 and 9999.

To calculate the bulls and cows, 

## Solution
```python
import random

secret_number = str(random.randint(1000, 9999))
print("Guess the number. It contains 4 digits.")

remaining_try = 7

def get_bulls_cows(number, user_guess):
   bulls_cows = [0,0] #cows, then bulls
   for i in range(len(number)):
       if user_guess[i] == number[i]:
           bulls_cows[0] += 1
       elif user_guess[i] in number:
           bulls_cows[1] += 1
   return bulls_cows

while remaining_try > 0:
   player_guess = input("Enter your guess: ")
  
   if player_guess == secret_number:
       print("Yay, you guessed it!")
       print("YOU WIN.")
       break
   else:
       bulls_cows = get_bulls_cows(secret_number,player_guess)
      
       print("Bulls: ",bulls_cows[0])
       print("Cows: ",bulls_cows[1])

       remaining_try -= 1

       if remaining_try < 1:
           print("You lost the game.")
           break
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
After solving the Bulls and cows for 2 digits, this one should become easier for you. 

However, solving this one by using if-else that we did for 2 digit bulls and cows game will become very harder. 

That's why we created the get_bulls_cows function. Inside that, we created a loop. For each digit, check the digit in the same place. 


&nbsp;
[![Next Page](../assets/next-button.png)](Word-completion.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`