## Reverse a string (recursion)

## The problem 
Reverse a string using a recursive function.

## Hints
You already know the recursive function. So, it would be easier. 

Also, let’s talk a little bit about the range selector (also known as slicing).

For example, you want to select a range of elements. You can define a range by using colon inside the third bracket.

In the code below, you are selecting from position 3 to just before 7 position by writing str[3:7]

Similarly, you will get 3:11 to get elements from the 3rd index to 10th index. 

While selecting by index, you can skip the first number. In that case, it will start from the beginning. Similarly, if you skip the last number, then it will go to the end of the string.

If you skip both, you will get the full string.

```python
str ='Hello young Programmer'
print(str[3:7])
print(str[3:11])

print ('skip range index')

print(str[:11])
print(str[3:])

print(str[:])
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**


## Solution
```python
def reverse_recur(str):
   if len(str) == 0:
       return str
   else:
       return reverse_recur(str[1:]) + str[0]
 
str = input("Enter your string: ")
rev_str = reverse_recur(str)
print ('Reverse of your string: ', rev_str)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
In the recursive function, look at the else condition. We are selecting str[1:] 

This means we are selecting the string from the first index and send it recursively to the reverse_recur function. 

And  we are adding str[0] at the end. Here, str[0] is the first element. And you are adding at the end. 

This means you are adding the first element at the end. And if you keep doing it every time and add the first element at the last. You will create the reversed string.


## Smart Solution
There is a smarter and quicker solution to reverse a string.

I asked my grandma how the code below works. She didn't’ answered.  Instead, she sent a letter to Google through her private pigeon. 

```python
txt = "Welcome to the Jungle"
print(txt[::-1])
```
 
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**
 
## Quiz
How would you slide a string and get the first five characters?

1. Str[1:6]
2. Str[1:5]
3. Str[:5]


<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is: 3</p>
 </details>

## take Away
You can slice a string to get a part of the string. 
 

 
&nbsp;
[![Next Page](../assets/next-button.png)](Reverse-Number.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`

