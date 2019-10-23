# 11.2: Rock Paper Scissor

## The Problem
Build s simple Rock paper Scissor game. 

## Hint
You will write a lot of if-else. Think about it in a way that if the first player types rock, which one the second player should have picked to win the game. Otherwise, the second player will lose the game. 

If you are not familiar with Rock Paper Scissors, you might be living under a rock for a while. 

Don’t worry. You always have google. If you don’t know about the game, Google it.

## Solution
 
```python
def get_winner(p1, p2):
   if p1 == p2:
       return "It's a tie!"
   elif p1 == 'rock':
       if p2 == 'scissors':
           return "First player wins!"
       else:
           return "Second Player wins!"
   elif p1 == 'scissors':
       if p2 == 'paper':
           return "First player win!"
       else:
           return"Second player wins!"
   elif p1 == 'paper':
       if p2 == 'rock':
           return "First player wins!"
       else:
           return "Second player win!"
   else:
       return "Invalid input!"
      
player1 = input("First player: rock, paper or scissors: ")
player2 = input("Second Player: rock, paper or scissors: ")
 
print(get_winner(player1, player2))
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
We took 2 players' input. Send those to the get_winner function. Inside the function, first, we check whether both the player entered the same thing. Then it will become a tie. 

The next step is to check whether the first player entered the rock. Then we see the second player input. If the second player entered scissor, the second player is the winner. Otherwise, the first player is the winner 

We repeated this two more times. And checked whether the first player entered paper or scissor. And based on the first player input, we compared the second player’s input.

Now think for 5 minutes, is there any different way you could have written the if-else logic here. 

If you find a way, add a question here so that everyone can see your code.



&nbsp;
[![Next Page](../assets/next-button.png)](Cows-and-bulls.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`