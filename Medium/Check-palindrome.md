# 9.1 Check Palindrome 

## The problem

Check whether the string is a palindrome.


## Hint
A palindrome is a word, phrase, or sequence that reads the same backward as forwards. For example, the word- madam

If you read it backward it will be madam as well. Similarly, eye, rotor, kayak, racecar, level, etc. are palindromes.

To check a palindrome, just reverse the word or the phrase, and then check whether the reversed string is the same as the initial string. 

If both are the same, it will be a palindrome.

## Solution
```python
my_str = input('String to check: ')
rev_str = my_str[::-1]

if my_str == rev_str:
  print("It is palindrome")
else:
  print("It is not palindrome")
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
We used the shortcut method to get the reversed string. And then we compared using if-else. 

That's it. 

The problem might sound complicated at the beginning. However, if you know the technique, the solution could become easier. 

So, the more you explore, the more you try, the more shortcut trick you will master.


&nbsp;
[![Next Page](../assets/next-button.png)](Dictionary-of-cubes.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`

