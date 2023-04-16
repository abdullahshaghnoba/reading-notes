# Python Scope (global.nonlocal) And Big O notation.

---
## In Python, variable scope refers to the region of a program where a variable can be accessed. There are two types of variable scopes: local and global.

---
## Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both?

### answer: Local variables are defined within a function and are only accessible within that function. They are destroyed when the function returns. Global variables, on the other hand, are defined outside of any function and are accessible from any part of the program.

Here is an example:

x = 10  # global variable

def my_function():
    y = 5  # local variable
    print(x + y)  # access global variable within function

my_function()  # prints 15

print(x)  # prints 10

In this example, x is a global variable that can be accessed within the my_function() function, but y is a local variable that can only be accessed within the function. When my_function() is called, it prints the value of x added to y. x can also be accessed outside of the function, as it is a global variable.

---
## How do the global and nonlocal keywords work in Python, and in what situations might you use them?

### answer: In Python, the global and nonlocal keywords are used to modify variable scopes.

The global keyword is used to declare that a variable is a global variable, even if it is being assigned a value within a function. This allows the variable to be accessed and modified from anywhere in the program. 
Here is an example:

x = 10

def my_function():
    global x
    x = 5
    print(x)  # prints 5

my_function()

print(x)  # prints 5
In this example, x is a global variable that is modified within the my_function() function using the global keyword.

The nonlocal keyword is used to declare that a variable is not local to the current function, but rather is defined in the enclosing scope. This allows the variable to be accessed and modified from within nested functions. Here is an example:


def outer_function():
    x = 10

    def inner_function():
        nonlocal x
        x = 5
        print(x)  # prints 5

    inner_function()

    print(x)  # prints 5

outer_function()
In this example, x is a variable defined in the outer function outer_function(). The inner_function() modifies the value of x using the nonlocal keyword.

We use global and nonlocal keywords when we need to modify the value of a variable in an outer scope. However, it is generally recommended to minimize the use of global and nonlocal variables, as they can make code more difficult to read and debug. It's better to pass values as arguments to functions or return values from functions.

----

## In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis?
### answer: Big O notation is a mathematical notation used to describe the complexity of an algorithm in terms of its input size. It is important because it helps us analyze and compare the efficiency of different algorithms and choose the most appropriate one for a particular task.

----
## Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials?

### answer: you whould need the random library to generate the result of rolling a dice and then use a loop to do that for multiple time and with keeping an eye on the count you can calculate the propabilty of getting a specefic number
Here is an example:

import random

def roll():
    return random.randint(1,6)

def count(amount):
    count_ = 0

    for i in range(1, amount+1):
        if roll() == 3:
            count_ += 1
    return count_

print(count(10000))

## Things I want to know more about: None.