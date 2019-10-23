# 11.6: Word hangman [Premium]

## The problem
Create a word hangman game.

## Hint
The word hangman is a simple game. You will provide a word with the first letter. Rest of the letters will be blank. For example, 

`s_ _ _ _ _ _ _ _ _`

The player has to guess the letters in the word. And the player will guess one letter at a time. If the letter exists in the word, it will appear to the player. 

If the letter doesn’t exist in the word, it will be counted as a wrong try. 

If the player exceeds the number of the wrong tries, the player will lose.

Otherwise, the player will win. 

## Solution
```python
import random
 
def selected_a_word():
    words = ['working', 'hard', 'makes', 'things', 'easier', 'congrats', 'programming', 'hero']
    word = words[random.randint(0, len(words)-1)]
    return word
 
def get_blank_word(word):
    blank_word = word[0]
    for i in range(1, len(word)):
            blank_word += '_'
    return blank_word
 
def word_hangman(word, so_far, letter, try_left):
    bad_try = True
    for i in range(0, len(word)):
            if word[i] == letter:
                    so_far = so_far[:i]+letter+so_far[i+1:]
                    bad_try = False
    if bad_try is True:
            try_left -= 1
            print('Wrong Try Left: ', try_left)
    print('so far you got: ', so_far)
    if word == so_far:
            print('YAY!!! You Win')
    elif try_left == 0:
            print('Opps!!! You Lost')
    else:
     next_letter = input ('Enter your next letter: ')
     word_hangman(word, so_far, next_letter, try_left)
 
# play the game
word = selected_a_word()
clue_word = get_blank_word(word)
word_hangman(word, clue_word, word[0], 5)
```

## Explanation
Take a deep breather. Start reading the code. 

Reading other’s code and trying to understand will be a common activity for a programmer. 

So, practice it here. 

If you don't understand any line, feel free to ask us a question. 

&nbsp;
[![Next Page](../assets/next-button.png)](../Harder/Simple-Calculator.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`