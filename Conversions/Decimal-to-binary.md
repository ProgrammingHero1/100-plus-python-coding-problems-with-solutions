# 4.4: Decimal to Binary

## The Problem
Convert a decimal number to binary number. 

## Decimal vs Binary

The numbers that we use every day is called decimal number. A decimal number could have any of the 10 digits (0, 1, 2, 3, 4,5 6, 7, 8, 9). 

Hence, 232, 789, 176, 511, etc. are decimal numbers. 

Sometimes, decimal numbers are called 10-based numbers. Because you could have 10 different digits in your number. 

On the other hand, binary numbers use two digits (0 and 1). The word binary means two. And binary numbers use two digits. Just one and 0. Buy using these two digits binary number system can represent any numbers. 

Some example of binary numbers re 10001, 11101, 100001, etc. 
## Hints
To convert a decimal number to a binary number, you have to keep dividing the number by 2.

While dividing, you will keep the remainder. These remainders will be used to build a binary number. 

Then, reverse the order of the reminder, to get the binary number. 

##  Solution
I looked into the below code 7 times to understand. Still trying to figure it out...So, spend some time here to look at the code:

```python
def dec_to_binary(n):
	bits = []
	
	while n > 0:
		bits.append(n%2)
		n = n // 2
	bits.reverse()
	
	binary = ''
	for bit in bits:
		binary += str(bit)
	return binary


num = int(input("Your decimal number: "))
binary = dec_to_binary(num)
print("Your binary is:", binary)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
You have seen the remainder and dividing the number with // before. That is the core part of this decimal to a binary algorithm. 

So, this part should be easier for you:

```python
bits = [ ]
while n > 0:
	bits.append(n%2)
	n = n // 2
```

The reminder is n%2. And, the result(floor division) of dividing by two is n//2.

Rest is simple. 

You reverse the bits array by calling bits.reverse(). 

After reverse, you have the digits of the binary. To display the binary bits as one number, you can declare a string called binary. 

Then, run a for loop over your bits array and join the binary bit as a string. 

We used the str method to convert number to a string. If we didn’t convert the digit to a string, it will be added as a number. 

That’s why, '1'+'1'+'1'+'0'+'0'+'1' will become '111001'. If you didn’t convert each digit to string it will become 4 (1+1+1+0+0+1)

Try to read this explanation and code multiple times. And, if needed, come back again and again. We don’t expect you to understand everything in your first try. 

If you keep trying and revisiting , again and again, these will start making sense.


## Quiz

What is a binary number?
1. Numbers written on a trash bin
2. Numbers that use 0,1 only
3. Numbers with any 2 digits

<details>
 <summary><b>Show Answer</b></summary>
   <p>The answer is : 2</p>
 </details>

## Take Away
Binary numbers use 0 and 1 only. 



&nbsp;
[![Next Page](../assets/next-button.png)](Decimal-to-binary-recursive.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`
