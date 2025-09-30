# Queue_CPP

# Experiment 18 – Queue Implementation in C++

- **Name:** Gandluri Sai Tejas
- **PRN:** 24070123045
- **Class:** ENTC A2
- **Title:** Implementation of Queue using Array in C++

---

## Aim  
To implement a **Queue data structure** using arrays in C++ and perform basic operations such as **enqueue, dequeue, and display**.

---

## Objectives  
1. To understand the working of the **Queue** (FIFO: First In, First Out) data structure.  
2. To implement **Queue operations** (insertion, deletion, display) using arrays.  
3. To study **overflow and underflow conditions** in queues.  
4. To analyze the limitations of a simple queue and understand its use cases.  
5. To strengthen the concepts of **object-oriented programming (OOPs)** using classes in C++.  

---

## Theory  

A **Queue** is a linear data structure that follows the **FIFO (First In, First Out)** principle. The element that is inserted first is the one that gets removed first. This makes it different from stacks (which follow LIFO).

### Key Concepts:
- **Front:** Refers to the index of the element that will be removed first (oldest element).  
- **Rear:** Refers to the index where the next element will be inserted.  
- **Enqueue (Insertion):** Adds an element to the rear of the queue.  
- **Dequeue (Deletion):** Removes an element from the front of the queue.  
- **Display:** Shows all the elements currently present in the queue.  

### Characteristics of Queue:
1. **Sequential Access:** Elements are processed in the order they arrive.  
2. **Restricted Operations:** Insertion happens only at the rear, deletion only from the front.  
3. **Overflow Condition:** When the queue is full, no more elements can be inserted.  
4. **Underflow Condition:** When the queue is empty, no element can be deleted.  

### Types of Queues:
1. **Simple Queue (Linear Queue):** Insertion from rear, deletion from front.  
2. **Circular Queue:** Overcomes the wastage of space in linear queues.  
3. **Priority Queue:** Elements are dequeued based on priority, not order.  
4. **Deque (Double Ended Queue):** Insertion and deletion from both ends.  

This experiment focuses on **Simple Queue implementation using arrays**.

---

## Comparison: Stack vs Queue

| Feature           | Stack (LIFO)            | Queue (FIFO)            |
|-------------------|-------------------------|--------------------------|
| Insertion         | Top                     | Rear                     |
| Deletion          | Top                     | Front                    |
| Order of Access   | Last In, First Out      | First In, First Out      |
| Use Cases         | Function calls, Undo    | Scheduling, Buffering    |

---
# Program Summary
## Algorithm  

1. **Start**  
2. Initialize `front = -1`, `rear = -1`.  
3. **Enqueue (value):**  
   - If `rear == SIZE - 1`, print **Overflow**.  
   - Else increment `rear`, insert element at `arr[rear]`.  
   - If `front == -1`, set `front = 0`.  
4. **Dequeue():**  
   - If `front == -1 OR front > rear`, print **Underflow**.  
   - Else delete element from `arr[front]` and increment `front`.  
5. **Display():**  
   - If queue is empty, print message.  
   - Else traverse from `front` to `rear` and display elements.  
6. Perform operations as per `main()`.  
7. **End**.  

---

## Program Summary  
- Implemented a **Queue class** with private members `arr`, `front`, and `rear`.  
- Defined **enqueue**, **dequeue**, and **display** functions.  
- Tested the queue in the `main()` function with a set of operations.  
- Successfully demonstrated **FIFO operation** and handled **overflow/underflow conditions**.  

---

## Concepts Used  
- **Object-Oriented Programming (OOPs):** Encapsulation via class and methods.  
- **Data Structures:** Queue using arrays.  
- **Control Structures:** Conditional statements (`if-else`) to handle overflow/underflow.  
- **Loops:** For traversal during display.  
- **Macros:** `#define SIZE 5` for queue size.  

---

## Conclusion  
This experiment helped in understanding the **queue data structure** and its implementation using arrays in C++.  

We observed:  
- **FIFO principle** in action.  
- How **overflow** occurs when the array is full.  
- How **underflow** occurs when trying to remove from an empty queue.  
- Practical usage of **class-based encapsulation** in C++.  

Queues are widely used in real-life applications such as:  
- **CPU scheduling**  
- **Printer queue management**  
- **Buffering in networks**  
- **Task scheduling systems**  
