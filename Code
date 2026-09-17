# TASK 2: A SIMPLE CALCULATOR WITH BASIC ARITHMETIC OPERATIONS

# imorting the logo from art.py
from art import logo

# introdicing the functions for addition
def add(n1, n2):
  return n1 + n2

# introdicing the functions for subtraction
def subtract(n1, n2):
  return n1 - n2

# introdicing the functions for multiplication
def multiply(n1, n2):
  return n1 * n2

# introdicing the functions for division
def divide(n1, n2):
  return n1 / n2

# operations dictionary to map the symbols to their corresponding functions
operations = {
'+': add, 
'-': subtract,
'*': multiply,
'/': divide,
}

# defining the calculator function
def calculator():
  print(logo)

  num1 = float(input("What is the first number: "))
  run = True
  while run: 
    for e in operations:
      print(e)
    oprsel = input("Type a math operation: ") 
    num2 = float(input("What is the next number: "))

    calculation = operations[oprsel]
    answer = calculation(num1, num2)

    print(f"{num1} {oprsel} {num2} = {answer}")
    print(f"Type 'y' to continue calculating with {answer}, type 'n' to exit or type 'new' for a new calculation")
    continue_calc = input("Type y/n/new: ")
    if continue_calc == 'y':
      run = True
      num1 = answer
    elif continue_calc == 'n':
      run = False
      print("\nGoodbye.")
    elif continue_calc == 'new':
      calculator()
    else:
      print("Invalid response.")
      run = False
      print("\nGoodbye.")
calculator()
