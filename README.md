# 100 Plus Python Coding Problems With Solutions
---

### 1.1: User input to Number

**S-1: The problem**

Take two inputs from the user. One will be an integer. The other will be a float number. Then multiply them to display the output.

<details>
   <summary><b>S-2: Click Here For Show Hints</b></summary>
   <p>Use input. By default, input gives you a string. Then use int and float to convert the input to a number. And then multiply them. <br><br>That’s it.</p>
 </details>
<br>

#### S-3: Solution

```python
int_text = input("Give me an integer number: ")
int_num = int(int_text)
float_text = input("Give me a float  number: ")
float_num = float(float_text)
result = int_num * float_num
print("Your result is: ", result)
```

**[Try It:](/#)**


#### S-4: Shortcut

> You wrote input in one line and then in the next line you used int or float to convert the number. You can write the two lines in one line. Like below 

```python
int_num = int(input('Give me an integer number: '))
float_num = float(input('Give me a float  number: '))
result = int_num * float_num
print('Your result is: ', result)
```

**[Try It:](/#)**
&nbsp;
#### S-5: Going Forward

Going forward, we will write input and conversion in one line.

#### S-6: Quiz

Which one is used to convert string to a number?


1. number
2. convert
3. int or float

**The answer is: 3**


*S-7: Take Away*

Use int or float to convert user input to a number.
&nbsp;
###### tags: `programmig-hero` `python` `float` `int`


![NEXT PAGE](/assets/next-button.png)
[![Next Page](/assets/next-button.png)](/Easy-ones/Math-Power.md)