# 🔄 Types of Queue-Circular Queue in Python

This project demonstrates the implementation of a **Circular Queue** in Python. The queue accepts 3 user values, performs enqueue and dequeue operations, and displays the removed values.

---

## 🎯 Aim

To develop a Python program that implements a Circular Queue:
- Accepts 3 values from the user
- Removes the 3 values from the queue
- Displays the removed values

---

## 🧠 Algorithm

1. **Initialize** a circular queue of fixed size (e.g., 5).
2. **Define the following functions**:
   - `enqueue()`: Inserts an element into the queue.
   - `dequeue()`: Removes an element from the queue.
   - `display()`: Shows the queue contents.
3. Accept 3 values from the user using the `enqueue()` method.
4. Remove 3 values using the `dequeue()` method.
5. Print the removed values.

---

## 💻 Program:

```
# Circular Queue Implementation

class CircularQueue:
    def __init__(self, size):
        self.size = size
        self.queue = [None] * size
        self.front = -1
        self.rear = -1

    # Enqueue operation
    def enqueue(self, value):
        if (self.rear + 1) % self.size == self.front:
            print("Queue is Full")
            return

        if self.front == -1:
            self.front = 0

        self.rear = (self.rear + 1) % self.size
        self.queue[self.rear] = value

    # Dequeue operation
    def dequeue(self):
        if self.front == -1:
            print("Queue is Empty")
            return None

        value = self.queue[self.front]

        if self.front == self.rear:
            self.front = self.rear = -1
        else:
            self.front = (self.front + 1) % self.size

        return value


# Main program
cq = CircularQueue(5)
removed = []

# Accept 3 values
for i in range(3):
    val = input("Enter value: ")
    cq.enqueue(val)

# Remove 3 values
for i in range(3):
    removed_value = cq.dequeue()
    if removed_value is not None:
        removed.append(removed_value)

# Display removed values
print("Removed values:", removed)

```

### Output:


<img width="403" height="150" alt="image" src="https://github.com/user-attachments/assets/88e91638-01c6-451a-8f0e-72f8d422acbe" />


## Result:

The program is exucted successfully and the output is verified
