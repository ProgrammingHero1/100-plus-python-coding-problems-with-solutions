# 11.5:  Word Completion [premium]

## The Problem
Build a simple word completion game. 

You will be given a partial word with hyphens. It’s a clue to an actual word. For example, 

-a-e

Now you have to provide a word that matches with the exposed letters. If you provide any of these words- “game” or “fame” or “lame”, your answer will be correct. 

Because all these words have the letter “a” in the second position and the letter “e” in the fourth position. 

So, the idea is, your provided word has to have the same letter as the clue. 

S-2: hint
You have to write a function that takes the clue word with hyphens and the provided answer. 

Then check whether the provided answer has the same letters in the same position as the clue word.

And you can ignore the position with hyphens. Because the user can put any letter there.



## Solution

```python
import random
 
def get_a_clue():
   clues = ['-a-e', 'y-ll-w', 's-mm-r', 'wi-t-r','s-n-y', 'l-v-','-i-e']
   position = random.randint(0, len(clues)-1)
   clue = clues[position]
   return clue
 
def check_word_match(clue, guess):
   if len(clue) != len(guess):
            return False
   for i in range (len(clue)):
       if clue[i] != '-' and clue[i ]!= guess[i]:
           return False
   return True
 
# start the game
word_clue = get_a_clue()
print('Your word clue:', word_clue)
answer = input('What would be the word: ')
 
is_matched = check_word_match(word_clue, answer)
 
if is_matched is True:
    print('WOW!!! You win')
else:
    print('Opps! you missed it.')
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**


## Explanation

We have two functions here. 

The first one is providing a clue. We have a list of clues. Under that, we generate a random position. 

Inside the randint function, you may notice that the second parameter is len(clues) -1. 

Let’s say you have a list with 5 elements. The length of the list is 5. However, as the index starts from 0. The index of the last element will be 4. It will start at 0. And the positions are 0, 1, 2, 3, 4. 

That’s why, if the len of the list is 5, the index of the last element will be 4. That is 5-1. Hence you see  len(clues) - 1.


We have another function, check_word_match. In that function, we are taking two parameters, clue and the guess. 

If the length of the clue and the length of the guess is not equal. We are sure that your guess is not correct. Because the clue and the guess should have the same number of elements. 

After that, we check the letters without hyphens for each position. That’s why we need a for loop. 

In the place of hyphens, there could be any letter. Hence, you have to match the letter with non-hyphens. That’s why the if has two conditions. 

The first condition is to check whether it is not a hyphen. The second condition is to check whether the letter in the clue matches with the letter of the guess. If the letter doesn’t match, this means your guess doesn’t match with the exposed characters in the clue.

That’s why we return False immediate. 

Otherwise, the for loop will finish and you will return True at the end of the function. 

Code underneath the function should be easier for you.

## Quiz

What should be the highest index of a list using len? 

```python
nums = [12, 56, 34, 71, 23, 17]

len(nums)
len(nums) +1
len(nums) - 1

The answer is: 3
```


&nbsp;
[![Next Page](../assets/next-button.png)](Word-hangman.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`