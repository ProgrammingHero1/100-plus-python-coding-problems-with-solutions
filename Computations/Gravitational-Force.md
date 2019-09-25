## 6.4 Gravitational Force

### S-1: The Problem
Compute gravitational force between two objects. 

### S-2: Hint
The formula for gravitational force is 

**F = G m1m2/r2**

Here G is the gravitational constant. Its value is 6.673*10-11

So, take three input from the users. The mass of the first object, the mass of the second object and the distance between them.  

### S-3: Solution

```python
mass1 = float(input("First mass: "))
mass2 = float(input("Second mass: "))
 
r = float(input("Distance between the objects: "))
 
G = 6.673*(10**-11)
force =(G*mass1*mass2)/(r**2)
 
print("The gravitational force is:", round(force, 5),"N")
```
 
**[Try It:](/https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

### S-4: Explanation
The calculation is simple. Only two things need to be learned from this. 

**Have a look, how we wrote 6.673*10-11**

> Also, note that while displaying the force, we used a round function. In the round function, we passed the force, the variable we want to display. Then we passed another parameter to tell, how many decimal points we want to display. 


&nbsp;
[![Next Page](../assets/next-button.png)](Triangle-Area.md)
&nbsp;

###### tags: `programmig-hero` `python` `float` `int` `math`
