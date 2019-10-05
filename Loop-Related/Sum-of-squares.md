
## 3.3 Sum of squares

#### S-1: The problem
Take a number as input. Then get the sum of the numbers. If the number is n. Then get

02+12+22+32+42+.............+n2

<details>
 <summary><b>S-2: Click Here For Show Hints</b></summary>
   <p>Once again, run a for loop with a range. Inside the loop, use the power of 2. Then add that power to a sum variable. That’s it. </p>
 </details>
<br>

#### S-3: Solution
```python
def square_sum(num) :
    sum = 0
    for i in range(num+1) :
        square = (i ** 2)
        sum = sum + square
    
    return sum

num = int(input('Enter a number: '))
sum = square_sum(num)

print('sum of square numbers is ', sum)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

#### S-4: Explanation
This one is super easy. You declared a variable sum with an initial value 0.

Then you run a for loop. This loop will run for range (num +1). 

The reason we are running it until num + 1. Because, we know that the range will stop just before the number inside it. 

For example, if we want to run the loop including 10. We should write 11 inside the range function. 

If needed, go to the code editor and run the following code. 

```python
for i in range(10):
	print(i)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**
And then run
```python
for i in range(11):
	print(i)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**


#### S-5: Shortcut
Sometimes there could be a better and easier way to solve a problem. For example, there is a simple math formula to calculate the sum of the square. 

This is the reason, you should search online and learn from different sources. This will make you  stronger and better. 

If you want to calculate the sum of the square of n numbers, the formula is-

n*(n+1)(2*n+1)/6

Now you can use this formula.
```python
def sum_of_square2(n):
    sum = n*(n+1)*(2*n+1)/6
    return sum

num = int(input('Enter a number: '))
sum = sum_of_square2(num)
print('Your sum of Square is: ', sum)
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

#### S-6: Quiz

Why you should learn problem-solving from multiple sources?

1. To utilize the internet bill correctly
2. To learn alternative solutions
3. To pretend that you are busy 

**The answer is: 2**

#### S-7: Take Away
Knowing shortcut ways will make you smarter and faster.

&nbsp;
[![Next Page](../assets/next-button.png)](Second-Largest.md)
&nbsp;

###### tags: `programmig-hero` `python` `float` `int` `math`

