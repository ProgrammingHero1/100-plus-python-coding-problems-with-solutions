# Reverse word order

## The problem
Reverse the word in a sentence. 

For example, if the input string is “Hello young Programmer”, the output will be “Programmer young Hello”

## Hints
There are two methods that you can call on a string. One is called split(). If you don’t pass any parameter to this function, it will split the string by whitespace. 

The opposite of split is join. You can write what you want to join string by. And then pass the array to it. 

For example, if you want to join a list elements by whitespace, you can write the whitespace and then join like bellow

```python
str ='Hello young Programmer'
words = str.split()
print(words)

together = ' '.join(words)
print(together)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Solution
 
```python
def reverse_words(sentence):
   words = sentence.split()
   words.reverse()
   return " ".join(words)
 
usr_input = input("Enter a sentence: ")
reverse = reverse_words(usr_input)
print('Reversed words are: ', reverse)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
Once you understand the split and the join method, this code should become super easy for you. 

If you have any confusion, let us know. 

## Quiz

What is the purpose of the split method on a string?

1. Breakdown string into elements of a list
2. Split the string if it has no whitespace
3. Adds some splitting characteristics

<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is: 1</p>
 </details>


## Quiz
How would you split a string by the character a?

1. str.split()
2. str.split(“ ”)
3. str.split(‘a’)

<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is: 3</p>
 </details>

## Quiz

How would you join each string in the words list by the hyphen(-)?
1. words.join(“-”)
2. words.split(“-”)
3. “-”.join(words)

<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is: 3</p>
 </details>

## Reverse domain

Let’s say, you have the website name www.programming-hero.com

Now you want to reverse the domain name: com.programming-hero.www

```python
site='www.programming-hero.com'
parts = site.split('.')
parts.reverse()
rev =  '.'.join(parts)
print(rev)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**
Alternatively, you can write the whole code in one line. 

```python
site='www.programming-hero.com'
rev = '.'.join(reversed(site.split('.')))
print(rev)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## take Away
The split method breaks string into elements of a list.



&nbsp;
[![Next Page](../assets/next-button.png)](../Medium/Check-palindrome.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`

