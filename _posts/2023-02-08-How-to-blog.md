---
layout: post
title: "How to Order a List with a For Loop"
author: Brannon Olive
description: A brief description on how to take a list of numbers and order them from least to greatest or greatest to least.
image: 
---

## How to Order a List of Numbers
The goal of this post is to show you how to take a list of integers and order them from least to greatest or greatest to least by using a for loop. This same idea will work for other programming languages. You will just have to change the syntax to match whatever language you decide to use. In the example I will be be doing, I will be using Python and ordering the list from least to greatest. I know that Python has a sort function that can do this, but this will help with other languages and if there is a case where the built in function does not work.

1. You need a list of unordered integers (if you are using a different, a similar data structure will work) \n
    x = (6,1,7,8,3,2)
2. Now you will want to initial the for loop to the length of the list. \n
    for i in range(len(x)):
3. Next you will want to create a nested for loop that starts one iter ahead of the outside loop. \n
    for j in range(i+1, len(x):
4. This is where you want to start checking whether a one value is bigger than the next. To do this, you check if the value at x[i] is bigger than the value at x[j]
    if x[i] > x[j]:
5. Inside of this if statement is where the swapping of values occurs. If x[i] is bigger, you want to swap the values. To do this, you need to store one in a temporary variable, change that value to the other indexed values, and then use the temporary variable to change the other index.
    y = x[i]
    x[i] = x[j]
    x[j] = y
These are all of the steps that you need to sort the list. When you put them all together, it looks like this.
    for i in range(len(x)):
    for j in range(i+1, len(x)):
        if(x[i] < x[j]):
            y = x[i]
            x[i] = x[j]
            x[j] = y
            
Following these steps will sort the list. To do this but reverse the order, you would just change the greater than to a less than in the if statement. 
