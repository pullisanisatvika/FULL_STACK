# Java Foundations Week 1

This repository contains my Week 1 Java programming foundation practice.

The goal of this week is to understand the basic building blocks of Java programming and build a complete console-based calculator application.

---

## Goal

By the end of this week, I should be able to:

- Create and use variables
- Understand primitive and reference data types
- Take input from the user
- Print output to the console
- Use arithmetic, comparison, and logical operators
- Write conditional statements
- Write loops
- Create and call functions
- Understand basic scope
- Understand stack and heap memory at a beginner level
- Understand primitive vs reference types
- Write simple recursive functions
- Build a complete console calculator app

---

## Recommended Daily Study Time

| Task | Time |
|---|---:|
| Learn concept | 45–60 min |
| Code examples | 45–60 min |
| Exercises | 60–90 min |
| Review | 20–30 min |

---

## Topics Covered

### Day 1 — Variables, Data Types, and Output

Topics covered:

- Variables:
  Variables acts as a container that could store values. For example,
    int age = 25;
    double height = 6.1;
    String name = "Harish";
    boolean isStudent = true;
  Considering java, Java is strongly typed. That means every variable must have a data type.For example, (int marks = 90;),     where,int is the datatype, marks is the variable name and 90 is the value.
- Primitive data types
- `String`
- Output using `System.out.println()`
- Combining text and variables
- Basic naming rules

Exercises completed:

- Print personal details
- Student marks program
- Product bill program

---

### Day 2 — Operators and User Input

Topics covered:

- Arithmetic operators
- Comparison operators
- Logical operators
- Integer division
- User input using `Scanner`
- Common Scanner methods:
  - `nextInt()`
  - `nextDouble()`
  - `next()`
  - `nextLine()`

Exercises completed:

- Add two numbers
- Area of rectangle
- Simple interest calculator
- Check adult status

---

### Day 3 — Conditional Statements

Topics covered:

- `if`
- `if-else`
- `else-if`
- `switch`
- Input validation using conditions
- Menu-based logic

Exercises completed:

- Even or odd checker
- Positive, negative, or zero checker
- Grade calculator
- Simple menu program

---

### Day 4 — Loops

Topics covered:

- `for` loop
- `while` loop
- `do-while` loop
- `break`
- `continue`
- Repeating user input

Exercises completed:

- Print numbers from 1 to 100
- Print even numbers from 1 to 50
- Multiplication table
- Keep asking until user enters 0
- Sum of numbers from 1 to N

---

### Day 5 — Functions and Scope

Topics covered:

- Creating functions
- Calling functions
- Parameters
- Return values
- `void`
- Variable scope
- Splitting code into reusable blocks

Exercises completed:

- Add function
- Even or odd function
- Function that returns boolean
- Grade function
- Basic calculator functions

---

### Day 6 — Memory, Call Stack, References, and Recursion

Topics covered:

- What memory is
- Stack memory
- Heap memory
- References
- Primitive types vs reference types
- Function call stack
- Recursion
- Base case
- Recursive call

Exercises completed:

- Predict output with primitive variables
- Predict output with arrays
- Recursive countdown
- Recursive factorial

---

### Day 7 — Mini Project: Console Calculator App

The final project for Week 1 is a console-based calculator application.

Features:

- Addition
- Subtraction
- Multiplication
- Division
- Divide-by-zero handling
- Invalid menu choice handling
- Invalid input handling
- Repeats until the user exits
- Uses separate functions for each operation

---

## Project Structure

```text
java-foundations-week-1
├── day-01-variables
│   └── Main.java
├── day-02-operators-input
│   └── Main.java
├── day-03-conditions
│   └── Main.java
├── day-04-loops
│   └── Main.java
├── day-05-functions
│   └── Main.java
├── day-06-memory-recursion
│   └── Main.java
└── day-07-calculator-app
    └── Main.java
