# 11.3: Cows and Bulls (2 digits)

## The Problem
Create a Cows and Bulls game.

## Hints
The Cows and Bulls is a number guessing game. In this game, the user guesses a number. Usually, the number will be a 4 digit number. However, here we will try with 2 digits number first.

So, if the user guesses the number correctly, he/she will win. If they didn’t guess the exact number, then you will calculate the bulls and cows. 

Let’s say the number is: 8529

And your guess is: 3428

If you guess any position digit currently, you will get a bull. For your guess, you didn’t match the first, second or the last digit. However, you guess the 3rd digit correctly. Hence your bulls will be 1.

On the other hand, if one or more digits of the secret number exist in your guess, you will get a cow. 

In summary, if you matched the digit with the position, you will get a bull. On the other hand, if you have the digit in a different place, it will cows. 

In the above guess, you have 8 in the 4th position. The 8 exists in the secret number in a different location, that's why you will get 1 cow. 

Hence your score will be: 
Bulls: 1
Cows: 1
 

Another example-
Secret number: 4271 
player's try: 1234
Answer: 1 bull and 2 cows. (The bull is "2", the cows are "4" and "1".)


## Solution
```python
import random
 
secret_number = str(random.randint(10, 99))
print("Guess the number. It contains 2 digits.")
 
remaining_try = 7
 
while remaining_try > 0:
   player_guess = input("Enter your guess: ")
   
   if player_guess == secret_number:
       print("Yay, you guessed it!")
       print("YOU WIN.")
       break
   else:
       bulls = 0
       cows = 0
      
       if player_guess[0] == secret_number[0]:
           bulls += 1
       if player_guess[1] == secret_number[1]:
           bulls += 1
       if player_guess[0] == secret_number[1]:
           cows += 1
       if player_guess[1] == secret_number[0]:
           cows += 1
 
       print("Bulls: ",bulls)
       print("Cows: ",cows)
 
       remaining_try -= 1
 
       if remaining_try < 1:
           print("You lost the game.")
           break
```
 
## Explanation
In the beginning, we created a secret number. Then asked the user to guess the number. Also, we set the variable remaining_try to 7. 

This means we allow the player to guess the number 7 times. If he/she guesses the correct number within 7 tries, he/she will win. Otherwise, lose.

We ran the while loop for remaining_try. If the user’s guess is correct, we say you win.

Otherwise, we start counting bulls and cows. For that purpose, we start at 0 bulls and 0 cows. 

For bulls, we check whether the first digit in the secret_number matches with the player’s guessed number. If it matches, we increase the bulls by 1. 

Also, check the 2nd digit of the secret number with the player’s guess. If that matches, we increase the bulls by 1. 

For cows, we check whether the first digit of the secret number matches with the second digit of the player guess. Increase cows by 1. Similarly, if the 2nd digit matches with the first digit of the guess number, increase cows by 1. 

In summary, bulls are guessed digit matches for the same position in the secret number. And cows are the digits that match in any other position other than the current position. 

Then we display the bulls and cows. 

Finally, if there is no remaining try (remaining try < 1), print that user lost.


&nbsp;
[![Next Page](../assets/next-button.png)](Cows-and-bulls(4digits).md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`