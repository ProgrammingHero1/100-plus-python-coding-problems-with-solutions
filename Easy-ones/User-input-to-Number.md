# 100 Plus Python Coding Problems With Solutions
---

# User input to Number

##  The problem
Take two inputs from the user. One will be an integer. The other will be a float number. Then multiply them to display the output.

## Hints
Use input. By default, input gives you a string. Then use int and float to convert the input to a number. And then multiply them. That’s it.

## Solution
```python
int_text = input("Give me an integer number: ")
int_num = int(int_text)
float_text = input("Give me a float  number: ")
float_num = float(float_text)
result = int_num * float_num
print("Your result is: ", result)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Shortcut
> You wrote input in one line and then in the next line you used int or float to convert the number. You can write the two lines in one line. Like below 

```python
int_num = int(input('Give me an integer number: '))
float_num = float(input('Give me a float  number: '))
result = int_num * float_num
print('Your result is: ', result)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Going Forward
Going forward, we will write input and conversion in one line.

## Quiz
Which one is used to convert string to a number?

1. number
2. convert
3. int or float

<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is : 3</p>
 </details>

## Take Away*

Use int or float to convert user input to a number. <br>

&nbsp;
[![Next Page](../assets/next-button.png)](Math-Power.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`
