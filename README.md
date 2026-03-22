Here is a clean, well-structured **README** you can use for your C deadlock detection program:

---

# 📄 Deadlock Detection in Operating System (C Program)

## 📌 Overview

This project implements a **Deadlock Detection Algorithm** in C.

It determines whether a system is in a **deadlock state** based on the current allocation of resources, outstanding requests, and available resources.

The program simulates how an Operating System checks for deadlocks among multiple processes.

---

## 🧠 Concept

A **deadlock** occurs when a set of processes are blocked because each process is holding a resource and waiting for another resource held by another 

process.

This program uses:

* **Allocation Matrix** → Resources currently allocated to processes

* **Request Matrix** → Resources still needed by processes

* **Available Vector** → Resources currently available

---

## ⚙️ Algorithm Used

The program follows the **Deadlock Detection Algorithm**:

1. Initialize all processes as **unfinished**.

2. Search for a process whose request is less than or equal to available resources.

3. If found:



   * Mark the process as finished

   * Release its allocated resources back to available pool

5. Repeat until no more processes can proceed.

6. If any process remains unfinished → **Deadlock exists**.

---

## 📥 Input Requirements

The program requires the following inputs:

1. **Number of Processes (n)**

2. **Number of Resource Types (m)**

3. **Allocation Matrix (n × m)**

4. **Request Matrix (n × m)**

5. **Available Resources (m values)**

---

## ▶️ How to Compile and Run

### Step 1: Compile

```bash
gcc deadlock.c -o deadlock
```

### Step 2: Run

```bash
./deadlock
```

---

## 📊 Example

### Input

```
Enter number of processes: 3
Enter number of resource types: 3

Allocation Matrix:
0 1 0
2 0 0
3 0 2

Request Matrix:
0 0 0
2 0 2
0 0 0

Available Resources:
0 0 0
```

### Output

```
Processes in Deadlock:
P1 
Deadlock Detected!
```

---

## 📌 Features


* Detects deadlock in multi-process systems

* Supports multiple resource types

* Identifies specific processes involved in deadlock

* Simple and efficient implementation

---

## ⚠️ Limitations

* Does **not prevent deadlock** (only detects it)

* Assumes correct input from user

* Uses fixed maximum size (`MAX = 10`)


---

## 🚀 Possible Improvements

* Dynamic memory allocation instead of fixed arrays

* Graphical visualization of resource allocation

* Integration with **Banker’s Algorithm** for deadlock avoidance

* Input validation and error handling

---

## 👨‍💻 Author

Developed as part of **Operating Systems coursework** to demonstrate deadlock detection techniques.

---
Wakoli ian Wangila

Kirinyaga University

Bsc Computer Science

https://github.com/wakoli001
* Or **comment your C code line-by-line for submission**
# OS-deadlock
