# learning how to read and write files in Python is crucial for data manipulation, analysis, and management. It is a fundamental skill that every Python programmer should master in order to become proficient in data processing and analysis.

## What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?

### answer : it helps with automatic close of the file properly after the work is done on it which prevents errors and memory leaks.

## Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method? 

### answer : 'read()' reads the entire file at once while 'readline()' reads a specific line at a time, so if you need to read the whole file 'read()' would do it but if you need to read a piece of the file 'readline ()' is the method for it note that you can use 'readline()' to read the whole file as pieces which is more efficient considering the memory needed to execute the command and it gives better chance to process the data.

## Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example?

### answer : exceptions are a mechanism in python to handle runtime errors that might happen during the execution of a program, 'try' contains a block of code that will be executed and might throw an error, 'except' contains a block of code with the way to handle the said error, 'finally' contains a block of code the will be executed regardless, ex : 
try:
    x = int(input("Enter a number: "))
    y = 10 / x
    print("Result:", y)
except ZeroDivisionError:
    print("you can't divide by zero!")
finally:
    print("End of program !!")  


## Things I want to know more about : None    