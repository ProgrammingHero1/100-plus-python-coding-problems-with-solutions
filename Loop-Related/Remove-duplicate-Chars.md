
## Remove duplicate characters

## The problem
For a given string, remove all duplicate characters from that string.

## Hints
Create a result string. Then loop through the string and check whether the current character not in the string. If it is not, then add it. Otherwise, it’s already there adding it will make it duplicate.

## Solution
```python
def remove_duplicate(your_str):
   result = ''
   for char in your_str:
       if char not in result:
           result += char
   return result
 
user_input = input('what is your string:')
 
no_duplicate = remove_duplicate(user_input)
print('Without duplicate: ', no_duplicate)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
We just created a function. In the function, we are taking a string as an input. 

Inside the function, we created a variable named result with initial value as an empty string. 

Our task is to loop through the input string and then for each character/letter check whether the character (char) not in the result. If it is not in the result, we add it to the result string. 

If it is already added in the result string, we don’t add it to it. Because, if we add it again, it will become a duplicate.

So, the overall task is very simple. 

If needed, go to the code playground type the code multiple times and you will understand it. 

## Quiz
How would you check whether a character exists in a string? 

1. not in
2. ==
3. index

<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is : 1</p>
 </details>

## Take Away
The not in is just the opposite check of in.


&nbsp;
[![Next Page](../assets/next-button.png)](../Conversions/Miles-to-Kilometers.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`

