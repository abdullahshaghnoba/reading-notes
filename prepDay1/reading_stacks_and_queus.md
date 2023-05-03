# Topic: Stacks and Queues in Python

## analogy:
Imagine a stack of books and a queue of people waiting in line. A stack represents a collection of items where new items are added on top, and the most recent item is the first one to be removed (Last-In-First-Out). On the other hand, a queue represents a line of people where new people join at the end, and the first person to join is the first one to be served (First-In-First-Out).

## detail in depth:
Let's dive deeper into stacks. A stack is a data structure that follows the LIFO principle. It consists of two primary operations: push and pop. The push operation adds an item to the top of the stack, while the pop operation removes and returns the topmost item. The top represents the position where the next pop or push will occur. Stacks can be implemented using lists in Python, where the end of the list represents the top of the stack.

## WHY, WHAT, HOW:

**WHY**: Stacks are useful when you need to keep track of a sequence of items and want to access the most recently added item quickly. They are efficient for handling function calls, undo/redo operations, and parsing expressions.

---

**WHAT**: A stack is a collection of items that follows the Last-In-First-Out (LIFO) principle.

---

**HOW**: In Python, you can create a stack using a list. To add an item to the stack, use the append() method, and to remove an item, use the pop() method.
Tutorial / Walk through an example:
Let's create a stack in Python and perform some operations:

python
Copy code
# Create an empty stack
stack = []

# Push items onto the stack
stack.append('A')
stack.append('B')
stack.append('C')

# Print the stack
print("Stack:", stack)

# Pop an item from the stack
popped_item = stack.pop()
print("Popped item:", popped_item)

# Print the updated stack
print("Stack:", stack)
Output:


Stack: ['A', 'B', 'C']
Popped item: C
Stack: ['A', 'B']

---

Quiz:

What is the primary principle behind a stack?
a) First-In-First-Out (FIFO)
b) Last-In-First-Out (LIFO)
c) Random access
d) None of the above

Which operation adds an item to the top of the stack?
a) push
b) pop
c) append
d) remove

What data structure can be used to implement a stack in Python?

a) list
b) tuple
c) dictionary
d) set

(Answers: 1 - b, 2 - a, 3 - a)

Vocabulary/Definition list:

Stack: A data structure that follows the LIFO principle, where items are added and removed from the top.
Push: An operation that adds an item to the top of the stack.

---

Pop: An operation that removes and returns the topmost item from the stack.
LIFO: Last-In-First-Out, a principle followed by stacks.
List: A built-in data structure in Python that can be used to implement a stack.
Cheat sheet:

---

Creating a stack: stack = []

---

Adding an item to the stack: stack.append(item)

## Things I want to know more about : None.