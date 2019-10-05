## 6.5 Triangle Area
---

### S-1: The Problem 
Take three sides of a triangle. And then calculate the area of the triangle. 

### S-2: How it works 
To calculate the area of the triangle. First, calculate the half of the perimeter. Here perimeter is the sum of each side of the triangle.

Let’s call it s. 

Then you have to perform square root of the formula like below-

```python
s = (a+b+c)/2
area = √(s(s-a)*(s-b)*(s-c))
```

### S-3: the code
```python
import math

a = float(input('Enter first side: '))
b = float(input('Enter second side: '))
c = float(input('Enter third side: '))

# calculate the semi-perimeter
s = (a + b + c) / 2

# calculate the area
area = math.sqrt(s*(s-a)*(s-b)*(s-c))
print('Area of your triangle is ', area)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

### S-4: Explanation
To calculate the square root. We used the math module. And call math.sqrt. 

```python
import math
print ( math.sqrt(4) )
```

This will give you 2 as output.

Similarly, math.sqrt(25) will give 5 as output.

This is something new you have learned this time. 

### S-5: Quiz

1. How would you calculate the square root of a number. 
2. Use math.square.root
3. Use math.sqroot
4. Use math.sqrt

**The answer is: 3**

### S-6: Take Away
The math module has a lot of math-related functionalities. 


&nbsp;
[![Next Page](../assets/next-button.png)](..README.md)
&nbsp;

###### tags: `programmig-hero` `python` `float` `int` `math`
