# Python Fundamentals: Scenario-Based Programming Exercises

## Overview

This repository contains a Google Colab notebook (`Copy_of_Python_Day_2_Exercises_Mitchel_.ipynb`) that serves as a practical exploration of fundamental Python programming concepts through a series of scenario-based exercises. This project demonstrates my ability to apply core programming constructs to solve real-world problems, showcasing logical thinking, problem-solving skills, and proficiency in foundational Python syntax.

## Objective

The primary objective of this notebook was to solidify understanding and practical application of essential Python programming elements. By the end of these exercises, the following capabilities were reinforced:

* ✅ Use conditional statements (`if`, `elif`, `else`) to control program flow.
* ✅ Apply the modulus operator (`%`) to check number properties like divisibility and parity.
* ✅ Implement input validation and string comparisons for basic user authentication.
* ✅ Use `while` loops to repeat tasks based on conditions or attempt limits.
* ✅ Combine loops and decision-making logic to build interactive programs (e.g., simple menus).
* ✅ Practice using `for` loops with the `range()` function for efficient number iteration.

## Key Skills Demonstrated

* 🐍 **Core Python Programming:** Strong grasp of fundamental Python syntax and structure.
* 💡 **Algorithmic Thinking:** Designing step-by-step solutions to defined problems.
* 🧩 **Conditional Logic:** Effective use of `if`, `elif`, and `else` for decision-making.
* 🔄 **Iterative Processes:** Implementing `for` and `while` loops for repetitive tasks and program control.
* ➕ **Mathematical Operations:** Application of arithmetic and modulus operators for numerical computations.
* ✍️ **Function Definition:** Creating reusable code blocks with custom functions.
* ⌨️ **User Interaction:** Handling user input (`input()`) and providing clear output (`print()`).
* 🐛 **Problem Solving:** Breaking down complex scenarios into manageable programming tasks.

## Project Exercises & Python Syntax Insights

This notebook features a series of practical challenges, each designed to highlight specific Python functionalities:

### 1. Security Door Access

**Scenario:** Implement a security system that grants or denies access based on a secret code.

**Python Syntax:**
```python
passcode = 123
user_entry = int(input("Please enter today's passcode:"))

if user_entry == passcode:
  print("Access Granted, Welcome")
elif user_entry != passcode:
  print("Access Denied, Incorrect Code")
```
**Techniques & Insights:**
* **`input()` function:** Used to receive user input.
* **`int()` conversion:** Converts string input to an integer for numerical comparison.
* **`if`/`elif` statements:** Demonstrates basic conditional logic for decision-making. This is a foundational concept for controlling program flow.

### 2. Number Divisibility Checker

**Scenario:** Build a tool to check if a number is divisible by both 3 and 7.

**Python Syntax:**
```python
user_entry = int(input("Please enter a number:"))
if user_entry % 3 == 0 and user_entry % 7 == 0:
  print("The number is divisible by both 3 and 7")
else:
  print("The number is not divisible by both 3 and 7")
```
**Techniques & Insights:**
* **Modulus operator (`%`):** Used to determine divisibility (remainder is 0).
* **Logical `and` operator:** Combines multiple conditions, requiring both to be true.
* **`else` statement:** Provides an alternative path when the `if` condition is false. This exercise highlights precise conditional checking.

### 3. Simple Calculator Tool

**Scenario:** Develop an interactive calculator that allows users to perform basic arithmetic operations repeatedly until they choose to exit.

**Python Syntax:**
```python
print("This is a calculator app.")

while True:
  number1 = float(input("Enter first number: "))
  number2 = float(input("Enter second number:"))

  print("Please choose operation")
  choice = int(input("Press 1:addition, 2:subtraction, 3:multiplication, 4:division, 5:exit"))

  if choice == 1:
    addition = number1 + number2
    print(addition)
  elif choice == 2:
    subtraction = number1 - number2
    print(subtraction)
  elif choice ==3:
    multiplication = number1 * number2
    print(multiplication)
  elif choice == 4:
    division = number1 / number2
    print(division)
  elif choice ==5:
    print("Thank you for using the app.")
    break
```
**Techniques & Insights:**
* **`while True` loop:** Creates an indefinite loop, allowing the calculator to run continuously.
* **`break` statement:** Exits the `while` loop when the user chooses to exit.
* **Nested `if`/`elif`:** Manages multiple operation choices within the loop.
* **`float()` conversion:** Handles decimal numbers for calculations. This demonstrates building interactive, menu-driven applications.

### 4. Fitness Tracker: Sum of Steps

**Scenario:** Calculate the total number of steps if steps increase by one each day up to a user-specified number.

**Python Syntax:**
```python
user_entry = int(input("Please enter a positive number:"))
total = sum(range(1, user_entry + 1))
print(total)
```
**Techniques & Insights:**
* **`range()` function:** Generates a sequence of numbers, commonly used with loops or `sum()`.
* **`sum()` function:** Efficiently calculates the sum of all numbers in an iterable. This showcases concise problem-solving using built-in functions.

### 5. Math Quiz App: Prime Number Checker

**Scenario:** Determine if a user-entered positive integer is a prime number.

**Python Syntax:**
```python
def is_prime(n):
    if n <= 1:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True

user_entry = int(input("Please enter a positive number:"))
if is_prime(user_entry):
  print("The number is a prime number")
else:
  print("The number is not a prime number")
```
**Techniques & Insights:**
* **Function Definition (`def`):** Encapsulates logic into a reusable function, promoting modular code.
* **Optimized Loop for Primes:** The loop iterates only up to the square root of `n` (`n**0.5`), demonstrating an understanding of basic algorithmic optimization for efficiency.
* **Conditional `return` statements:** Efficiently exits the function once a condition is met. This highlights structured programming and basic algorithm design.

## Tools and Environment

* 🐍 **Python:** The core programming language used for all exercises.
* ☁️ **Google Colab:** The cloud-based Jupyter notebook environment used for developing and executing the code, facilitating interactive learning and accessibility.

## Conclusion

This Python Fundamentals notebook serves as a strong testament to my foundational programming skills. Through these scenario-based exercises, I've demonstrated proficiency in conditional logic, iterative structures, function creation, and user interaction. These capabilities are essential for building robust applications and lay a solid groundwork for more advanced data analysis and software development tasks.

---


