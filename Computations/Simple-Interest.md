## 6.1: Simple Interest 

---

### S-1: The Problem
You borrowed $5000 for 2 years with 2% interest per year.
Calculate the simple interest to know how much you have to pay?

### S-2: Hint
Just take amount, duration and interest rate. 

You have to multiply these three. And, don’t forget: you have to convert percent to a fraction by dividing it by 100.

### S-3: The Solution

```python
principle = int(input("Money you borrowed: "))
interest_rate = float(input("Interest Rate: "))
time = float(input("Overall Duration: "))

# Calculates simple interest
simple_interest = principle * (interest_rate/100) * time

print("Simple interest is:", simple_interest)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

### S-4: Explanation
Read the code. I think you don’t need any extra explanation here. 


&nbsp;
[![Next Page](../assets/next-button.png)](Complex-Interest.md)
&nbsp;

###### tags: `programmig-hero` `python` `float` `int` `math`
