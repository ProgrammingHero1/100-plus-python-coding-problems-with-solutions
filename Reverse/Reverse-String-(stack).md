# 8.2 Reverse a string (stack)

## The Problem 
Reverse a string using a stack.

## Hint
This is a little fancier way to reverse the string. However, this will help you understand one concept called stack. 

If you are not familiar with the stack. Don’t worry. We have it covered in the Data Structure galaxy. 

For now, just remember, you have to use .pop() method to get the last element of the list. 

## Solution
```python
def reverse_stack(str):
  # Create an empty stack (list to use as stack)
  stack = []
   # Push all characters of string to stack
  for char in str:
      stack.append(char)
  # Pop all characters of string
  # and add it to the rev
  rev = ''
  while len(stack) > 0:
       last = stack.pop()
       rev = rev + last
       # print(last, rev)
       
  return rev
usr_str = input('What is your string:')
reverse = reverse_stack(usr_str)
print('Reversed is: ', reverse)
```

**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
In the function, we declared a list named stack. And then we loop through the input string and put every character of the string inside the list. 

Then we have an empty string. 

Later we ran a while loop. Inside the while loop, we used the .pop() method to get the last element of the list. 

Then we added the last element to the reverse string. 

The overall idea is very simple, take the last element and add keep adding it. 

Hence, the last element will come first and you will put it in the first position. And then, in the next iteration, the second to the last element will be coming and will get added. 

If needed, add a print command to see how it works.

&nbsp;
[![Next Page](../assets/next-button.png)](Reverse-String-(recursive).md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`

