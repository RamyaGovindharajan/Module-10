# # Stack-Stack Reversal Program 🔁

This Python program demonstrates how to reverse the values in a stack using basic stack operations like push and pop.

## 🎯 Aim

To write a Python program that reverses the values in a stack using standard stack operations.

## 📋 Algorithm

1. Create an empty stack.
2. Read an integer `n` from the user (number of elements to push).
3. Loop `n` times:
   - Read an integer from the user.
   - Push it onto the stack.
4. Create an empty list called `reverse`.
5. While the stack is not empty:
   - Pop the top element.
   - Append it to `reverse`.
6. Print the reversed list.


### Program:

```
# Stack Reversal Program

stack = []

# Step 2: Read number of elements
n = int(input("Enter number of elements: "))

# Step 3: Push elements into stack
for i in range(n):
    value = int(input("Enter value: "))
    stack.append(value)

# Step 4: Create reverse list
reverse = []

# Step 5: Pop all elements and store in reverse list
while len(stack) != 0:
    reverse.append(stack.pop())

# Step 6: Print reversed stack
print("Reversed stack:", reverse)

```


## 🧪 Sample Input and Output:


<img width="453" height="202" alt="image" src="https://github.com/user-attachments/assets/480ae8ec-ea58-4931-8d6a-c7f047c57017" />


## Result:

The program is exucted successfully and the output is verified

