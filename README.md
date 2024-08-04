# codtechitsolutions-internship
• Title : CodeTech IT Solutions Internship - Task Documentation: Simple Calculator with Advance Features

• *Intern Information:* 
    #Name: Md. Ammaar Quadri
    #Intern ID : COD4479

![Logo] (https://github.com/maq765/codtechitsolutions-internship/blob/raw/main/logo.jfif)

# Python Calculator Documentation

## Introduction

Welcome to the comprehensive documentation for the Python Calculator project. This documentation aims to provide a detailed explanation of the code, its functionality, and user interactions. The Python Calculator is a simple yet versatile calculator program implemented in Python. It supports basic arithmetic operations such as addition, subtraction, multiplication, and division, along with advanced features like exponentiation. Users can interact with the calculator through a command-line interface, making it accessible and easy to use.

## Features

- Supports addition, subtraction, multiplication, division, and exponentiation.
- Provides a user-friendly command-line interface for interaction.
- Handles invalid inputs gracefully with appropriate error messages.
- Allows users to quit the program at any time.

## Getting Started

To use the Python Calculator, follow these steps:

1. **Download the Code**: Obtain the Python script containing the calculator code.
2. **Run the Script**: Execute the Python script using a Python interpreter.
3. **Follow On-Screen Instructions**: Interact with the calculator by following the on-screen menu.

## Code Explanation

Below is a detailed explanation of the code structure and functionality:

```python
# Importing the math module for exponentiation
import math

# Function Definitions for Arithmetic Operations
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y != 0:
        return x / y
    else:
        return "Error: Cannot divide by zero"

def exponentiate(x, y):
    return x ** y

# Main Calculator Function
def calculator():
    # Display Menu Options
    print("Simple Calculator with Advanced Features")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Exponentiation")
    print("6. Quit")

    # User Interaction Loop
    while True:
        choice = input("Enter choice (1-6): ")

        # Quit Option
        if choice == '6':
            print("Exiting the calculator. Goodbye!")
            break

        # Arithmetic Operations
        if choice in ('1', '2', '3', '4', '5'):
            try:
                num1 = float(input("Enter first number: "))
                num2 = float(input("Enter second number: "))
            except ValueError:
                print("Error: Please enter valid numbers.")
                continue

            if choice == '1':
                result = add(num1, num2)
                print("Result: ", result)
            elif choice == '2':
                result = subtract(num1, num2)
                print("Result: ", result)
            elif choice == '3':
                result = multiply(num1, num2)
                print("Result: ", result)
            elif choice == '4':
                result = divide(num1, num2)
                print("Result: ", result)
            elif choice == '5':
                result = exponentiate(num1, num2)
                print("Result: ", result)
        else:
            print("Invalid choice. Please enter a number between 1 and 6.")

# Entry Point for Execution
if __name__ == "__main__":
    calculator()
```

## Conclusion

This documentation has provided a comprehensive overview of the Python Calculator project, including its features, code explanation, and user interactions. With its simple yet powerful functionality, the Python Calculator serves as a useful tool for performing various arithmetic operations.  
