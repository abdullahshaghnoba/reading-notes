# TDD with Python : we need this path of working because it gives us the quality we need for the softwares we develop with great, readable and stable structure by building test units that satisfy our goals first

## What are the key principles of Test-Driven Development (TDD) in Python, and how do they contribute to the overall quality of code?

### The key principles of TDD in Python are writing tests before writing code, running tests frequently, and ensuring all tests pass before moving on to the next feature. TDD contributes to the overall quality of code by promoting a more systematic and rigorous approach to development, leading to fewer bugs and better-designed code.   

## Explain the purpose of the if __name__ == '__main__': statement in Python scripts. What are some use cases for including this conditional in your code?

### we use this statement to check if a Python file is being run as the main program, rather than being imported as a module into another program. This allows for conditional execution of code, such as running test code or initializing variables. Use cases include running standalone scripts and ensuring code is not executed when imported.

## Describe the concept of recursion in Python?

### recursion is a function that calls it self repetedly until a ceartin condition is satisfied, it might be direct or indirect calls, (the recursive function is a function that calls it self).

## What is the difference between Python modules and packages? Explain how to create, import, and use them in your Python programs?

### In Python, a module is a single file containing Python code, while a package is a collection of modules (sub-packages) organized in a directory hierarchy.
### To create a module, you simply write your code in a .py file. To create a package, you need to create a directory and put one or more modules (with init.py files) inside it.

### To import a module or package, you use the import statement followed by the name of the module or package. For example, to import a module named mymodule.py, you would write "import mymodule". To import a function or class from a module, you can use the from ... import statement.

### To use a module or package in your code, you simply call the functions or classes defined in it using dot notation. For example, if you have a function named "my_function" in your module, you can call it using "mymodule.my_function()". If you have a class named "MyClass" in a sub-package called "mypackage.subpackage", you can instantiate it using "mypackage.subpackage.MyClass()".

## Things I want to know more about

