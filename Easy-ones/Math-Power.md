
## 1.2: Math Power

**S-1: The problem**
Take two numbers from the users. Calculate the result of second number power of the first number.

<details>
   <summary><b>S-2: Click Here For Show Hints</b></summary>
   <p>To power, you will need to use two asterisks symbols (two multiplication symbols). For example 4 to the power 3 will be</p>
 </details>
<br>

**result = 4**3**


#### S-3: Solution

```python
base_num = int(input('Give me the base number: '))
power_num = int(input('Give me the power number: '))
result = base_num ** power_num
print('Your result is: ', result)
```

**[Try It:](/#)**
&nbsp;
#### S-4: Think Different
Python has a built-in function named pow [blue]. The pow is a short form of the word power. And you can pass 2 numbers to the pow function. It will give you the second number as a power of the first number. 


#### S-5: Alternative Solution
Python has a built-in function named pow [blue]. The pow is a short form of the word power. And you can pass 2 numbers to the pow function. It will give you the second number as a power of the first number. 

```python
base_num = int(input('Give me the base number: '))
power_num = int(input('Give me the power number: '))
result = pow(base_num, power_num)
print('Your result is: ', result)

```
**[Try It:](/#)**

&nbsp;
[![Next Page](../assets/next-button.png)](Random-Number.md)
&nbsp;

###### tags: `programmig-hero` `python` `float` `int` `math`

