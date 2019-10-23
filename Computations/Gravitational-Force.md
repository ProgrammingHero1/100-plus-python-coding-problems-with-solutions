# 6.4 Gravitational Force

## The Problem
Compute gravitational force between two objects. 

## Hint
The formula for gravitational force is 

`F = G m^1m^2/r^2`

Here G is the gravitational constant. Its value is 6.673*10-11

So, take three input from the users. The mass of the first object, the mass of the second object and the distance between them.  

## Solution

```python
mass1 = float(input("First mass: "))
mass2 = float(input("Second mass: "))
 
r = float(input("Distance between the objects: "))
 
G = 6.673*(10**-11)
force =(G*mass1*mass2)/(r**2)
 
print("The gravitational force is:", round(force, 5),"N")
```
 
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
The calculation is simple. Only two things need to be learned from this. 

`Have a look, how we wrote 6.673*10-^11`

Also, note that while displaying the force, we used a round function. In the round function, we passed the force, the variable we want to display. Then we passed another parameter to tell, how many decimal points we want to display. 


&nbsp;
[![Next Page](../assets/next-button.png)](Triangle-Area.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`