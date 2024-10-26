# PYTHON_FUNCTIONS

Exploring Python functions: a collection of examples demonstrating function creation, parameters, default values, and variable scope.

# What does the len() function do in Python?

The `len()` function in Python returns the number of items in an object, such as strings, lists, tuples, dictionaries, and sets.
It returns an integer representing the size or length of these data structures.

# Write a code example using len() to find the length of a list.

list = [10, 20, 30, 40, 50]

print("LIST:",list)

print("Length of the list:", len(list))

![q1](https://github.com/user-attachments/assets/8ddaa58d-b458-4644-9187-b01c2759288f)

# Write a Python function greet(name) that takes a person's name as input and prints "Hello, [name]!"

def greet(name):

  print(f"Hello, {name}!")

user_name=str(input("Enter a Name: "))

greet(user_name)

![q2](https://github.com/user-attachments/assets/3bc1fcfa-b5a9-48b9-9f2b-991cffa78ba6)

# Write a Python function find_maximum(numbers) that takes a list of integers and returns the maximum value without using the built-in max() function. Use a loop to iterate through the list and compare values.

def find_maximum(numbers):

    if not numbers:
    
        return None
        
    maximum = numbers[0]
    
    for i in numbers:
    
        if i > maximum:
        
            maximum = i

    return maximum

numbers_list = [14, 29, 51, 8, 30]

print(numbers_list)

print("Maximum value:", find_maximum(numbers_list))

![q3](https://github.com/user-attachments/assets/378cf56f-735f-4ad5-bf3f-91dfd9d160a9)

# Explain the difference between local and global variables in a Python function.
  # Local Variables
  
  Scope: Defined inside a function; accessible only within that function.
  
  Lifetime: Exists only during the function's execution.
  
  Example:

def my_function():

    local_var = 10  # Local variable
    
    print(local_var)

my_function()  # This will print 10

print(local_var)  # This will raise an error,  local_var is not accessible here

![q4](https://github.com/user-attachments/assets/ed646b53-1bfc-43f4-a7b9-20db1f96ad70)

  # Global Variables
  
  Scope: Defined outside any function; accessible throughout the entire program.
    
  Lifetime: Exists for the duration of the program.
    
  Example:

global_var = 20  # Global variable

def my_function():

    print(global_var)  # Accessing the global variable

my_function()  # This will print 20

print(global_var)  # This will also print 20

![q5](https://github.com/user-attachments/assets/25961183-7ae2-4856-b407-8814614fd96d)

# Write a program where a global variable and a local variable have the same name and show how Python differentiates between them.

value = 10 # Global variable

def my_function():

    value = 5 # Local variable with the same name
    
    print("Inside the function, local value:", value)

my_function()

print("Outside the function, global value:", value)

![q6](https://github.com/user-attachments/assets/3984b95a-b7ea-4f39-8392-3d1c6f576953)

# Create a function calculate_area(length, width=5) that calculates the area of a rectangle. If only the length is provided, the function should assume the width is 5. Show how the function behaves when called with and without the width argument.

def calculate_area(length, width=5):

    area = length * width
    
    return area

area_with_width = calculate_area(10, 3)

print("Area with length and width:", area_with_width)

area_with_default_width = calculate_area(10)

print("Area with length and default width 5:", area_with_default_width)

![q7](https://github.com/user-attachments/assets/c0bce94a-0cb0-4e85-8e13-22ee710e6edd)









