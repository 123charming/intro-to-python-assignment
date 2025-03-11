# intro-to-python-assignment
Instructions:

Basic Calculator Program

Create a simple Python program that asks the user to input two numbers and a mathematical operation (addition, subtraction, multiplication, or division).
Perform the operation based on the user's input and print the result.
Example: If a user inputs 10, 5, and +, your program should display 10 + 5 = 15.
def simple_calculator():
  """
  A simple calculator program that performs basic arithmetic operations.
  """
  try:
    num1 = float(input("10 "))
    num2 = float(input("5"))
    operation = input("Enter the operation (+, -, *, /): ")

    if operation == '+':
      result = num1 + num2
      print(f"{num1} + {num2} = {result}")
    elif operation == '-':
      result = num1 - num2
      print(f"{num1} - {num2} = {result}")
    elif operation == '*':
      result = num1 * num2
      print(f"{num1} * {num2} = {result}")
    elif operation == '/':
      if num2 == 0:
        print("Error: Division by zero is not allowed.")
      else:
        result = num1 / num2
        print(f"{num1} / {num2} = {result}")
    else:
      print("Invalid operation. Please enter +, -, *, or /.")

  except ValueError:
    print("Invalid input. Please enter valid numbers.")

if __name__ == "__main__":
  simple_calculator()
