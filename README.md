# My-first-project

hey this is my first project.

print("Simple 4-Operation Calculator")
try:
    num1 = int(input("Enter the first number: "))
    op = input("Enter an operator (+, -, *, /): ")
    num2 = int(input("Enter the second number: "))

    if op == '+':
        res = num1 + num2
    elif op == '-':
        res = num1 - num2
    elif op == '*':
        res = num1 * num2
    elif op == '/':
        if num2 == 0:
            res = "Error: Division by zero is not allowed."
        else:
            res = num1 / num2
    else:
        res = "Invalid operator, Please use +, -, *, or /."

    print(res)

except ValueError:
    print("Invalid input. Please enter numeric values.")
