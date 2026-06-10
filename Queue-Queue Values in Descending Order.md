# Queue-Queue Values in Descending Order Using Python 🧮

This Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

## 🎯 Aim

To write a Python program to:
- Accept user inputs into a list (queue)
- Remove the first two elements (simulating dequeue)
- Display the remaining values in **descending order**

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` to determine how many elements will be added.
3. Loop `n` times:
   - Read an input value.
   - Append it to the list `q`.
4. Remove the first element using `pop(0)`.
5. Remove the second element using `pop(0)` again.
6. Sort the list in descending order.
7. Print the updated list.

## 🧪 Program: 

```
# Queue implementation using list

q = []

# Step 2: Read number of elements
n = int(input("Enter number of elements: "))

# Step 3: Input elements into queue
for i in range(n):
    value = int(input("Enter value: "))
    q.append(value)

# Step 4 & 5: Remove first two elements (if available)
if len(q) >= 2:
    q.pop(0)
    q.pop(0)
else:
    print("Not enough elements to remove two items.")

# Step 6: Sort in descending order
q.sort(reverse=True)

# Step 7: Print result
print("Remaining queue in descending order:", q)
```
### Output:

<img width="515" height="137" alt="image" src="https://github.com/user-attachments/assets/2306c725-ce9b-407f-9f7a-8f4feba6dd2f" />


## Result:

The program is exucted successfully and the output is verified
