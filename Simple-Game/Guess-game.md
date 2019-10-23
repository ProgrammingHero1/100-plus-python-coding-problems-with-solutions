# 11.1: Guessing Game

## The Problem
Build a simple guessing game where it will continuously ask the user to enter a number between 1 and 10.

If the user's guesses matched, the user will score 10 points, and display the score. 
If the users' guess doesn’t match display the generated number. 

Also, if the user enters “q” then stop the game. 

## Hints
This type of situation, where you don’t know how many times a user will try to make the guess. You have to use an infinity loop. And you will have a special condition to break the loop. 

The following is an infinity loop. 

```python
while True:
	print(True)
```

Also, to create a random integer number, you will need to import the random module. In the random module, you can call the randint to generate a random integer. Besides, you can enter two parameters. 

The first parameter will be the smallest number and the last number is the highest number.  Hence, every time you run the following code you will see a different number between 20 to 40.

```python
import random
 
rand = random.randint(20,40)
print(rand)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

The above code will generate a random number between 20 and 40. 

## Solution
```python
import random
print('To stop anytime, enter: q')
score = 0
while True:
  num = random.randint(0,10)
  guess = input("Guess a number between 0 to 10: ")
  if guess == 'q':
      print('Game Over.')
      break
  guess_num = int(guess)
  if guess_num is num:
      print('CONGRATS, you guessed it correctly')
      score += 10
      print('Your new score:', score)
  else:
      print('Your guess did not match')
      print('The number was:', num)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
Since we want to create a random number between 0 to 10 we used randint(0,10)

Also, we have special if. In that if, we compare whether user input is ‘q’. If it is the q, we break the while loop.

After that, we use the int to convert the user input to an integer number. We didn’t put the int directly on the user input. Because the user might enter q. And if you pass the q to the int method, it will throw an error. 

That’s why we put the int after the check for q. 

The bottom part of the code should be easier for you.


&nbsp;
[![Next Page](../assets/next-button.png)](Rock-paper-scissor.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`