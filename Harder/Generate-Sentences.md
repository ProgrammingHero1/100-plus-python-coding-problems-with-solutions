# 12.5: Generate Sentences [Premium]

## The Problem
You have three lists of words. Create all possible combinations of sentences by taking one element from each list.

## Hint
For each list, run a for loop for its len. This would be nested three for loops. 

Under the last loop, access elements from each loop and show them as output.

## Solution
```python
subjects=["I", "You"]
verbs=["Play", "Love"]
objects=["Hockey","Football"]
for i in range(len(subjects)):
   for j in range(len(verbs)):
       for k in range(len(objects)):
           print (subjects[i], verbs[j], objects[k])
```
**[Try it on Programming Hero](https://play.google.com/store/apps/details?id=com.learnprogramming.codecamp)**

## Explanation
It's simple...Just run three for loops for three lists you have, each one under another. And finally, under the last one, access all three.

Damn easy, isn't it?


&nbsp;
[![Next Page](../assets/next-button.png)](../User-Submitted/Simple-Clock.md)
&nbsp;

tags:  `programming-hero`  `python`  `python3`  `problem-solving`  `programming`  `coding-challenge`  `interview`  `learn-python`  `python-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`  `programming-contest`  `python-coding-challenges`  `python-problem-solving`