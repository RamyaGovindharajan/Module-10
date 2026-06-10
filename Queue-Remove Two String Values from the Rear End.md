# Queue-Remove Two String Values from the Rear End in Python 🧵

This Python program demonstrates how to manage a list of strings and remove the last two elements (i.e., from the rear of the list).

## 🎯 Aim

To write a Python program to:
- Accept `n` string values from the user
- Remove the last two values (rear end of the list)
- Display the updated list

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` from the user (number of strings).
3. Loop `n` times:
   - Read a string input.
   - Append it to the list `q`.
4. Remove the last element using `pop()`.
5. Remove the next last element using `pop()` again.
6. Display the updated list.

##  Program:

```
# Queue - Remove Two String Values from Rear End

q = []

# Step 2: Read number of elements
n = int(input("Enter number of strings: "))

# Step 3: Input strings into queue
for i in range(n):
    value = input("Enter string: ")
    q.append(value)

# Step 4 & 5: Remove last two elements (rear end)
if len(q) >= 2:
    q.pop()
    q.pop()
else:
    print("Not enough elements to remove two items.")

# Step 6: Display updated list
print("Updated list:", q)

```

### Output:

<img width="392" height="252" alt="image" src="https://github.com/user-attachments/assets/4d8bde05-63e1-43ff-b6df-7e4356db75e4" />


## Result:

The program is exucted successfully and the output is verified
