Java Foundations Week 1

This repository contains my Week 1 Java programming foundation practice.

The goal of this week is to understand the basic building blocks of Java programming and build a complete console-based calculator application.

⸻

Goal

By the end of this week, I should be able to:

* Create and use variables
* Understand primitive and reference data types
* Take input from the user
* Print output to the console
* Use arithmetic, comparison, and logical operators
* Write conditional statements
* Write loops
* Create and call functions
* Understand basic scope
* Understand stack and heap memory at a beginner level
* Understand primitive vs reference types
* Write simple recursive functions
* Build a complete console calculator app

⸻

Recommended Daily Study Time

Task	Time
Learn concept	45–60 min
Code examples	45–60 min
Exercises	60–90 min
Review	20–30 min

⸻

Topics Covered

Day 1 — Variables, Data Types, and Output

Topics covered:

* Variables
* Primitive data types
* String
* Output using System.out.println()
* Combining text and variables
* Basic naming rules

Exercises completed:

* Print personal details
* Student marks program
* Product bill program

⸻

Day 2 — Operators and User Input

Topics covered:

* Arithmetic operators
* Comparison operators
* Logical operators
* Integer division
* User input using Scanner
* Common Scanner methods:
    * nextInt()
    * nextDouble()
    * next()
    * nextLine()

Exercises completed:

* Add two numbers
* Area of rectangle
* Simple interest calculator
* Check adult status

⸻

Day 3 — Conditional Statements

Topics covered:

* if
* if-else
* else-if
* switch
* Input validation using conditions
* Menu-based logic

Exercises completed:

* Even or odd checker
* Positive, negative, or zero checker
* Grade calculator
* Simple menu program

⸻

Day 4 — Loops

Topics covered:

* for loop
* while loop
* do-while loop
* break
* continue
* Repeating user input

Exercises completed:

* Print numbers from 1 to 100
* Print even numbers from 1 to 50
* Multiplication table
* Keep asking until user enters 0
* Sum of numbers from 1 to N

⸻

Day 5 — Functions and Scope

Topics covered:

* Creating functions
* Calling functions
* Parameters
* Return values
* void
* Variable scope
* Splitting code into reusable blocks

Exercises completed:

* Add function
* Even or odd function
* Function that returns boolean
* Grade function
* Basic calculator functions

⸻

Day 6 — Memory, Call Stack, References, and Recursion

Topics covered:

* What memory is
* Stack memory
* Heap memory
* References
* Primitive types vs reference types
* Function call stack
* Recursion
* Base case
* Recursive call

Exercises completed:

* Predict output with primitive variables
* Predict output with arrays
* Recursive countdown
* Recursive factorial

⸻

Day 7 — Mini Project: Console Calculator App

The final project for Week 1 is a console-based calculator application.

Features:

* Addition
* Subtraction
* Multiplication
* Division
* Divide-by-zero handling
* Invalid menu choice handling
* Invalid input handling
* Repeats until the user exits
* Uses separate functions for each operation

⸻

Project Structure

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

⸻

Mini Project: Console Calculator App

Features

The calculator supports:

* Addition
* Subtraction
* Multiplication
* Division
* Exit option
* Input validation
* Error handling for division by zero

Sample Output

===== Calculator App =====
1. Addition
2. Subtraction
3. Multiplication
4. Division
5. Exit
Enter your choice: 1
Enter first number: 10
Enter second number: 20
Result: 30.0

⸻

Calculator App Code

import java.util.Scanner;
public class Main {
    public static double add(double a, double b) {
        return a + b;
    }
    public static double subtract(double a, double b) {
        return a - b;
    }
    public static double multiply(double a, double b) {
        return a * b;
    }
    public static double divide(double a, double b) {
        return a / b;
    }
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        boolean running = true;
        while (running) {
            System.out.println("\n===== Calculator App =====");
            System.out.println("1. Addition");
            System.out.println("2. Subtraction");
            System.out.println("3. Multiplication");
            System.out.println("4. Division");
            System.out.println("5. Exit");
            System.out.print("Enter your choice: ");
            if (!scanner.hasNextInt()) {
                System.out.println("Invalid input. Please enter a number from 1 to 5.");
                scanner.next();
                continue;
            }
            int choice = scanner.nextInt();
            if (choice == 5) {
                System.out.println("Exiting Calculator App...");
                running = false;
                continue;
            }
            if (choice < 1 || choice > 5) {
                System.out.println("Invalid choice. Please select between 1 and 5.");
                continue;
            }
            System.out.print("Enter first number: ");
            if (!scanner.hasNextDouble()) {
                System.out.println("Invalid input. Please enter a valid number.");
                scanner.next();
                continue;
            }
            double num1 = scanner.nextDouble();
            System.out.print("Enter second number: ");
            if (!scanner.hasNextDouble()) {
                System.out.println("Invalid input. Please enter a valid number.");
                scanner.next();
                continue;
            }
            double num2 = scanner.nextDouble();
            double result;
            switch (choice) {
                case 1:
                    result = add(num1, num2);
                    System.out.println("Result: " + result);
                    break;
                case 2:
                    result = subtract(num1, num2);
                    System.out.println("Result: " + result);
                    break;
                case 3:
                    result = multiply(num1, num2);
                    System.out.println("Result: " + result);
                    break;
                case 4:
                    if (num2 == 0) {
                        System.out.println("Error: Cannot divide by zero.");
                    } else {
                        result = divide(num1, num2);
                        System.out.println("Result: " + result);
                    }
                    break;
                default:
                    System.out.println("Invalid choice.");
            }
        }
        scanner.close();
    }
}

⸻

Week 1 Final Checklist

* I can create Java variables
* I can use int, double, char, boolean, and String
* I can print output
* I can take user input
* I can use arithmetic operators
* I can use comparison operators
* I can use logical operators
* I can write if-else conditions
* I can write switch statements
* I can write for loops
* I can write while loops
* I can write do-while loops
* I can create functions
* I can use parameters
* I can return values from functions
* I understand basic scope
* I understand stack vs heap at a beginner level
* I understand primitive vs reference types
* I can write basic recursion
* I completed the calculator app

⸻

Review Questions

1. What is a variable?

A variable is a named memory location used to store data.

2. What is the difference between int and double?

Type	Stores
int	Whole numbers
double	Decimal numbers

3. What is the difference between = and ==?

Symbol	Meaning
=	Assignment
==	Comparison

4. What is a loop?

A loop repeats a block of code while a condition is true.

5. What is a function?

A function is a reusable block of code that performs a specific task.

6. What is a return value?

A return value is the result sent back from a function.

7. What is scope?

Scope means where a variable can be accessed in a program.

8. What is stack memory?

Stack memory stores function calls and local variables.

9. What is heap memory?

Heap memory stores objects.

10. What is recursion?

Recursion is when a function calls itself.

⸻

Study Method Used

For each day, I followed this pattern:

1. Read the concept.
2. Type the example code manually.
3. Run the code.
4. Change values and observe the output.
5. Solve exercises without looking at the answer first.
6. Compare my solution with the answer.
7. Push the code to GitHub.

⸻

Final Outcome

After completing Week 1, I became more comfortable with Java basics, console input/output, conditions, loops, functions, memory basics, recursion, and building a simple menu-based console application.
