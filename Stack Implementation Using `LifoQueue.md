# Stack Implementation Using `LifoQueue` (Max Size 7) 🔄

This Python program demonstrates a stack implemented using the `LifoQueue` class from the `queue` module. It allows up to 7 elements, checks if the stack is full, and then prints the elements in reverse (LIFO) order.

## 🎯 Aim

To create a Python program that:
- Implements a stack using `LifoQueue` with a maximum size of 7
- Adds user-inputted values to the stack
- Checks whether the stack is full
- Prints the stack elements in reverse order (LIFO)

## 📋 Algorithm

1. Import the `LifoQueue` class from the `queue` module.
2. Create a stack with a maximum size of 7.
3. Read the number of elements (`n`) to be added to the stack.
4. Loop `n` times:
   - Read a value from the user.
   - Use `put()` to push it onto the stack if it's not full.
5. Use `full()` to check if the stack is full and print the result.
6. Use `get()` repeatedly to pop and print elements in reverse order.

## Program

```
from queue import LifoQueue

# Step 2: Create stack with max size 7
stack = LifoQueue(maxsize=7)

# Step 3: Read number of elements
n = int(input("Enter number of elements: "))

# Step 4: Push elements into stack
for i in range(n):
    value = input("Enter value: ")
    if not stack.full():
        stack.put(value)
    else:
        print("Stack is full! Cannot insert more elements.")
        break

# Step 5: Check if stack is full
print("Is stack full?", stack.full())

# Step 6: Pop and print elements in LIFO order
print("Stack elements in reverse order:")
while not stack.empty():
    print(stack.get())
```

## 🧪 Sample Input and Output:


<img width="492" height="277" alt="image" src="https://github.com/user-attachments/assets/af065aac-cde1-41ed-8f97-4d7dc31b42fe" />


## Result:

The program is exucted successfully and the output is verified
