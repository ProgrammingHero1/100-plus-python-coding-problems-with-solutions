# Smallest prime factor [premium]

## The problem
Find the smallest prime factor for the given number.

## Solution Hint
After finishing all the prime factors, this will be a piece of cake for you.

## Solution
```python
def get_smallest_factor(num):
   factor = 2
   while num % factor != 0:
       factor += 1
   return factor
 
num = int(input('Enter your number: '))
 
smallest_factor = get_smallest_factor(num)
 
print('The smallest prime factor is: ', smallest_factor)
```
 
## Explanation
Since we need only one factor. We can do it more easily. 

Just run a while loop. The condition of the loop is checking the remainder. If there is no remainder, the number got divided and you got the prime factor. If the remainder is not 0, then increase the factor by one.  


&nbsp;
[![Next Page](../assets/next-button.png)](..READMD.md)
&nbsp;

###### tags: `programmig-hero` `python` `float` `int` `math`