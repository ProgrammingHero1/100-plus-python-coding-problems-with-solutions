# 12.4: Permutation [Premium]
 
## The Problem
Find all permutation of a given list.

## Hints
In mathematics, the permutation is the way to find all possible order of elements 

For example, you have 1,2,3. Now all possible order is 
1,2,3
1,3,2
2,1,3
2,3,1
3,1,2
3,2,1

So, the permutation is a way to find all the possible order or sequence of elements.

Give me more: non-premium
One important part of the solution is to select one element and get a list excluding that element. Let's say you want to select the list without the 4th position element. 

All the elements before the 4th index element will be lst[:4]. This is from beginning to before the 4th element.

Similarly, all the elements after the fourth position will be lst[4+1:]. This is from the 4+1 or 5th element to the end.

This concept will help in permutation to select one element and place it in multiple places.

```python
lst = [2,3,4,6,11,16,7,8]
before = lst[:4]
after = lst[4+1:]
excluding = before + after
print(excluding)
print('-----------------------')
print(lst[:4] + lst[4+1])
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**


## Solution

```python
def get_permutation(lst):
   # For an empty list, there is no permutation
   if len(lst) == 0:
       return []
   # list with one element will have only one
   # permutation
   if len(lst) == 1:
       return [lst]
  # Create an empty list to store permutation
   perms = []
   for i in range(len(lst)):
       # Extract current elemnt from the list.
       current = lst[i]
       # Recursively call permutation for the
       # remaining list
       rem_list = lst[:i] + lst[i+1:]
       rem_perm = get_permutation(rem_list)
       # Generate permutations by adding first element
       for p in rem_perm:
           perms.append([current] + p)
   return perms
# now test the function
data = [1,2,3]
for perm in get_permutation(data):
   print (perm)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**


## Explanation
In the code, we are getting the current element by lst[i]. 
Then we create the remaining list by lst[:i] + lst[i+1:]

We stored it in the remaining list named as rem_list. After that, we recursively call the get_permutation. This will give permutation for the rest elements. We stored that in the rem_perm list.

Finally, we have to join the current element with the rest of the list. To do so, we have added [current] + p

The loop variable p is a list. Whereas the current is an element. You can not add 

3 + [2,1]

That’s why we put current in a list as well so that it becomes a list as well. In the following example,  

[3] + [2, 1]

This will create [3, 2, 1]. That’s why we did [current] + p  to make the final permutation. 

This code is harder. It will take a few practices to become comfortable with it.


&nbsp;
[![Next Page](assets/next-button.png)](Generate-Sentences.md)
&nbsp;

###### tags: `programmig-hero` `python` `float` `int` `math`