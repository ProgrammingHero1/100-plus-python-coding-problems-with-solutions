# 9.2: Cube Sum

## The Problem
With a given integral number n, write a program to calculate the sum of cubes.

## Hints
Cubes mean power of 3. Hence, the cube of 9 is 9**3.

Here you have to calculate the cube of a series. If you want to calculate the cube up to the number n. The series will look like- 

`1^3+2^3+3^3+4^3+ .. .. .. +n^3`

If you remembered the sum of the square, this one will be easier for you.

## The solution

```python
def cube_sum(num):
	sum = 0
	for n in range(num+1):
		sum = sum + n**3
	return sum


user_num = int(input('Enter a number: '))
result = cube_sum(user_num)
print('Your sum of cubes are: ', result)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Think Different
There is an alternative solution to calculate the sum of cube of the n numbers. You can use

`(n*(n+1)/2)^2`


## Alternative Solution

```python
n = int(input('Enter a number: '))
sum = (n*(n+1)/2)**2
print('Your sum of cubes are: ', sum)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Take Away
Sum of a series might have an easier formula.

&nbsp;
[![Next Page](../assets/next-button.png)](Armstrong-number.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`


