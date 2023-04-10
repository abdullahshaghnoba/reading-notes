# Classes and Objects And Thinking Recursively And Fixtures and Code Coverage
---
---
# Classes and objects are fundamental concepts in object-oriented programming, Classes and objects help organize and structure code, making it easier to manage and maintain, And Recursion is useful for solving problems that can be broken down into smaller subproblems.

---
## What are the key differences between classes and objects in Python, and how are they used to create and manage instances of a class?

### answer : Classes are blueprints or templates for creating objects, while objects are instances of a class, Classes and objects help organize and structure code, making it easier to manage and maintain, you can create an instances of a class by assigning it to an object then you can access the object.

---
## Explain the concept of recursion and provide an example of how it can be used to solve a problem in Python. What are some best practices to follow when implementing a recursive function?

### answer : Recursion is useful for solving problems that can be broken down into smaller subproblems, so it divides the problem into parts and apply the same behavior on them each time ex:
 def fibonacci (n):
    
    # Check if input is less than 0 then it will print incorrect input
    if n < 0:
        print("Incorrect input")
    # Check if n is 0 then it will return 0
    elif n == 0:
        return 0
    # Check if n is 1 it will return 1
    elif n == 1 :
        return 1
    # the rest of the numbers goes under this case
    else:
        return fibonacci(n-1) + fibonacci(n-2)
---

## What is the purpose of pytest fixtures and code coverage in testing Python code? Explain how they can be used together to improve the quality and maintainability of a project?

### answer :you use fixtures when you want to have some objects available to all of your tests, Those objects might contain data you want to share across tests, or they might involve the network or filesystem., code coverage shows the % that have been excuted of the code so you can make sure that by gitting 100% code coverage after running your test that all of your code have been excuted at least once / Fixtures help to ensure that tests run in a consistent environment, while code coverage helps to identify areas of your code that need testing and areas of your code that can be removed. By using these tools together, you can ensure that your code is well-tested, maintainable, and of high quality.