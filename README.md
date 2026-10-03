try:
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))

    print("\nChoose an operation:")
    print("+  Addition")
    print("-  Subtraction")
    print("*  Multiplication")
    print("/  Division")

    operation = input("Enter the operation (+, -, *, /): ")

    if operation == "+":
        print("Result:", num1 + num2)

    elif operation == "-":
        print("Result:", num1 - num2)

    elif operation == "*":
        print("Result:", num1 * num2)

    elif operation == "/":
        if num2 == 0:
            print("Error: Cannot divide by zero.")
        else:
            print("Result:", num1 / num2)

    else:
        print("Error: Invalid operation.")

except ValueError:
    print("Error: Please enter valid numbers.")
