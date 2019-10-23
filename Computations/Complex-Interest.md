# 6.2: Compound Interest

## The Problem
Take money borrowed, interest and duration as input. Then, compute the compound interest rate.

###   Hint
Compound interest formula is:
```python
A = P(1+r/100)t
```

Here, P is the principal amount; it is the amount that you borrowed. r is the interest rate in percentage and t is the time.

## Solution

```python
def compound_interest(principle, rate, time):
	interest = principle * ((1 + rate / 100) ** time)
	return interest

principle = int(input("Money you borrowed: "))
interest_rate = float(input("Interest Rate: "))
time = float(input("Overall Duration: "))

total_due = compound_interest(principle, interest_rate, time)

print("Interest Amount is:", total_due)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
Inside the function, just look into the power calculation. 

**(1 + rate / 100)  time**

Rest of the part should be easy for you. 

##  Take Away
To apply the same power on multiple things, put them inside parentheses and then apply the power. 


&nbsp;
[![Next Page](../assets/next-button.png)](Calculate-Grades.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`
