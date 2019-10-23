## Reverse a string

## The problem
Reverse a string. 

If the input is: Hello World.

The output should be: .dlroW olleH

## Hints
A string is almost like a list. A list of characters. You can access any element by index. You can run a for loop on it. You will get each character as an element. Besides, you can also add two string or join two characters


```python
my_string = "You are my Hero"
 
print('Access by index')
print('-------------')
print(my_string[0])
print(my_string[1])
print(my_string[4])
 
print('Run a for loop')
print('-------------')
for char in my_string:
   print(char)
 
print('now join strings')
print('-------------')
print('hello' + 'world')
print('h'+'w')
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

However, a string is not a list.

## Solution
 
```python
def reverse_string(str):
   reverse = ""
   for char in str:
       reverse = char + reverse
   return reverse
 
str = input("Enter your string: ")
result = reverse_string(str)
print(result)
```
 
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
A simple trick will make it work. 

Let’s say you wrote “Hello world.” if you break down it or run a for loop and get each character at a time. You will get first H and then e and then l … and so on.

Now, while adding each character add it before the previous one. 

Hence, first you will have H. then while adding e, you will add it before the H. It will become eH. 

Then “l” will come and add it before. This will give you-

leH

Keep doing it. And you will get

.dlroW olleH

Now if you look at the code you will understand why we did- 

reverse = char + reverse

## Quiz
What does it mean by the word immutable?
1. Immortal
2. Not changeable
3. Changeable


<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is: 2</p>
 </details>

## Quiz
Will you be able to append, remove or set a character to string by the index?

1. Yes
2. No
3. Sometimes

<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is: 2</p>
 </details>

## take Away
A string is an immutable ordered sequence. 


&nbsp;
[![Next Page](../assets/next-button.png)](Reverse-String-(stack).md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`
