# 9.3: Armstrong number. 

## The problem 
Check whether a number is an Armstrong number. 

## Armstrong number
Armstrong is a special number.

A number is an Armstrong Number or narcissistic number if it is equal to the sum of its own digits raised to the power of the number of digits.
 
Think about the number 371.  The total number of digits is 3. Now, for each digit, put the power of 3 and then add them. It will be:

```python
33 + 73 + 13 
= 27 + 343 + 1
= 371
```
Hence, 371 is an Armstrong number. 
 
Similarly, 1634 is another Armstrong number, because the total number of digits is 4. Now, power each digit and sum them. You will get the Armstrong number.
 
```python
= 14 + 64 + 34 + 44 
= 1 + 1296 + 81 + 256
= 1634
```


## The solution

```python
def check_armstrong(num):
	order = len(str(num))
	
	sum = 0
	
	# use temp to find each digit. Then power it
	temp = num
	while temp > 0:
		digit = temp % 10
		sum += digit ** order
		temp //= 10
	return num == sum
 
num = int(input('Enter your number: '))
 
if check_armstrong(num):
	print(num,"is an Armstrong number")
else:
	print(num,"is not an Armstrong number")
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
Three things could be new for you. 

First of all, to know the total number of digits in a number, we converted the number to a string. We used the str(num) to convert it to the string. And then we pass it to the len function. 

This mean, len function will tell you how many characters are on that string. 

Another thing we did is to store the input number in a temp variable. We had to do that because, while getting the digits, we are dividing the number by 10. 

However, at the end, we need to compare the result of the while loop in the sum with the original number. 

That's why, we set the num to the temp variable. And then, we divided the temp variable. In this way, the num variable remained the same. 

Finally, return num == sum means if num is equal to the sum, it will return True. Otherwise, it will return False. 

Hence, return num == sum is a shortcut method of:

```python
result = False
if num == sum:
    result = True
else: 
    result = False
return result
```


&nbsp;
[![Next Page](../assets/next-button.png)](Greatest-common-divisor.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`


