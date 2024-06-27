[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15337958&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

### Answer
- Python is a high-level, interpreted programming language known for its   simplicity, versatility, and readability.

Key Features:
- Readability: Python's syntax is clear and easy to understand, emphasizing readability and reducing the cost of program maintenance.

- Extensive Standard Library: Python comes with a large standard library that provides modules and packages for a wide range of tasks, from web development to data analysis and machine learning.

- Dynamically Typed: Python is dynamically typed, which means you don't need to declare variable types explicitly. This makes it quicker to write code and allows for faster iteration.

- Cross-platform: Python runs on various platforms such as Windows, macOS, and Linux, making it highly portable.

- Strong Community and Ecosystem: Python has a vibrant community that contributes to its ecosystem with libraries and frameworks, enhancing its capabilities in areas like web development (Django, Flask), scientific computing (NumPy, Pandas), and machine learning (TensorFlow, PyTorch).

Examples:
- Web Development: Frameworks like Django and Flask are popular for building scalable web applications.

- Data Science and Analytics: Libraries such as NumPy, Pandas, and Matplotlib facilitate data manipulation, analysis, and visualization.

- Machine Learning and AI: Python's simplicity and powerful libraries like TensorFlow and PyTorch enable developers to build and train machine learning models effectively.

Automation: Python's scripting capabilities make it ideal for automating repetitive tasks and system administration.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

### Answer:
Installing Python (Windows)
a. Download Python Installer:

- Go to the official Python website: python.org.
- Navigate to the Downloads section and click on the latest Python release suitable for Windows.
- Choose the installer based on your system architecture (32-bit or 64-bit).

b. Run Python Installer:

- Once the installer is downloaded, run the executable file (.exe).
- Check the box that says "Add Python to PATH" during the installation process.
- Click "Install Now" to start the installation.

c. Verify Installation:

- Open Command Prompt (cmd.exe) or PowerShell.
- Type 'python --version' or 'python -V' and press Enter.
- You should see the Python version number displayed, confirming a successful installation.

d. Set Up a Virtual Environment:

- Open Command Prompt or PowerShell.
- Install 'virtualenv' using pip (Python's package installer):

         pip install virtualenv
         Navigate to your project directory:

         cd path\to\your\project

- Create a virtual environment:

         python -m venv venv_name

- Replace 'venv_name' with the name you want for your 
virtual environment.

e. Activate the Virtual Environment:

- In Command Prompt or PowerShell, navigate to your project directory if not already there.
- Activate the virtual environment:
   - For Command Prompt:

         venv_name\Scripts\activate

   - For PowerShell:

         .\venv_name\Scripts\Activate.ps1

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

Answer:
print("Hello, World!")

   - The print() function in Python is used to output text or variables to the console. It accepts one or more arguments inside parentheses and prints them as output eg.

      print("Hello, World!")
   
   "Hello, World!" is a string literal enclosed in double quotes. It's the argument passed to the print() function, and it instructs Python to display "Hello, World!" on the console.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

Answer:
Basic Data Types in Python:
1. Integer (int):

Represents whole numbers without decimal points.
Example: x = 5

2. Float (float):

Represents numbers with decimal points.
Example: y = 3.14

3. String (str):

Represents sequences of characters enclosed in quotes (' or ").
Example: name = "John"

4. Boolean (bool):

Represents truth values True or False.
Example: is_python_fun = True

5. List (list):

Represents ordered collections of items, which can be of different types.
Example: numbers = [1, 2, 3, 4, 5]

6. Tuple (tuple):

Similar to lists but immutable (cannot be changed).
Example: coordinates = (10, 20)

7. Dictionary (dict):

Represents key-value pairs where each key maps to a value.
Example: person = {'name': 'Vijo', 'age': 30}

Example Script:

         # Define variables of different data types
         x = 10                 # Integer
         y = 3.14               # Float
         name = "Vijo"         # String
         is_python_fun = True   # Boolean
         numbers = [1, 2, 3]    # List
         coordinates = (10, 20) # Tuple
         person = {'name': 'Bob', 'age': 30}  # Dictionary

         # Print out the values and their types
         print(f"x: {x}, type: {type(x)}")
         print(f"y: {y}, type: {type(y)}")
         print(f"name: {name}, type: {type(name)}")
         print(f"is_python_fun: {is_python_fun}, type: {type(is_python_fun)}")
         print(f"numbers: {numbers}, type: {type(numbers)}")
         print(f"coordinates: {coordinates}, type: {type(coordinates)}")
         print(f"person: {person}, type: {type(person)}")

Output:

         x: 10, type: <class 'int'>
         y: 3.14, type: <class 'float'>
         name: Vijo, type: <class 'str'>
         is_python_fun: True, type: <class 'bool'>
         numbers: [1, 2, 3], type: <class 'list'>
         coordinates: (10, 20), type: <class 'tuple'>
         person: {'name': 'Bob', 'age': 30}, type: <class 'dict'>

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

Answer:
Conditional statements
- Conditional statements allow you to execute certain blocks of code based on conditions.

Example of an 'if-else' Statement:
         # Example of an if-else statement
         x = 10

         if x > 0:
            print("x is positive")
         else:
            print("x is zero or negative")

- x is assigned the value 10.
- The 'if' statement checks if x is greater than 0.
- If the condition (x > 0) evaluates to True, it executes the block of code indented under 'if'.
- Otherwise, if the condition is False, it executes the block indented under 'else'.

Loops:
- Loops in Python allow you to repeatedly execute a block of code. Two common types of loops are 'for' loops and 'while'  loops.

         # Example of a for loop
         numbers = [1, 2, 3, 4, 5]

         for num in numbers:
         print(num)

- The 'for' loop iterates over each element ('num') in the 'numbers' list.
- During each iteration, the current value of 'num' is printed.
- The loop continues until all elements in the 'numbers' list have been processed.

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

Answer:
Functions:
- Functions are reusable blocks of code that perform a specific task. They allow you to organize code into manageable pieces, improve code readability, and promote code reuse. 

            # Function that takes two arguments and returns their sum
            def sum_two_numbers(a, b):
               return a + b

            # calling the function
            num1 = 10
            num2 = 20
            result = sum_two_numbers(num1, num2)
            print(f"The sum of {num1} and {num2} is: {result}")
Output:

            The sum of 10 and 20 is: 30

Benefits of Functions:
a. Code Reusability: 
- Functions allow you to write code once and reuse it multiple times throughout your program.

b. Modularity: 
- Functions help break down complex tasks into smaller, manageable parts, improving code organization and readability.

c. Abstraction: 
- Functions hide the implementation details, making it easier to focus on what the code does rather than how it works.

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

Answer:
Differences:
A. Indexing:

- Lists: Elements are accessed by their index, starting from 0.
- Dictionaries: Elements are accessed by keys.

B. Order:

- Lists: Maintain the order of elements as they are inserted.
- Dictionaries: Do not guarantee any specific order; the order of key-value pairs may vary.

C. Mutability:

- Lists: Mutable; elements can be modified, added, or removed.
- Dictionaries: Mutable; values can be modified or new key-value pairs can be added or removed.

Sample Script:
         # Create a list of numbers
         numbers_list = [1, 2, 3, 4, 5]

         # Create a dictionary with key-value pairs
         person = {
            "name": "John",
            "age": 30,
            "city": "New York"
         }

         # Accessing elements
         print("List elements:")
         for num in numbers_list:
            print(num)

         print("\nDictionary elements:")
         for key, value in person.items():
            print(f"{key}: {value}")

         # Modifying elements
         numbers_list[0] = 10  # Change the first element in the list
         person["age"] = 31    # Update the age in the dictionary

         # Adding elements
         numbers_list.append(6)          # Add a new number to the list
         person["occupation"] = "Engineer"  # Add a new key-value pair to the dictionary

         # Removing elements
         numbers_list.remove(3)   # Remove the number 3 from the list
         del person["city"]       # Delete the 'city' key from the dictionary

         # Displaying modified lists and dictionaries
         print("\nModified List:")
         print(numbers_list)

         print("\nModified Dictionary:")
         for key, value in person.items():
            print(f"{key}: {value}")

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

Answer:
Exception handling:
- Allows you to manage and respond to errors that occur during program execution gracefully, rather than letting the program terminate abruptly. 

Eg.
            # Example: Division by zero handling

            try:
               num1 = int(input("Enter numerator: "))
               num2 = int(input("Enter denominator: "))
               
               result = num1 / num2
               print(f"Result of division: {result}")

            except ZeroDivisionError:
               print("Error: Division by zero is not allowed.")
               
            except ValueError:
               print("Error: Please enter valid integers.")

            finally:
               print("Execution completed. Closing resources if necessary.")

Try Block ('try'): 
- Is used to enclose the code that you anticipate might throw an exception. If an exception occurs within this block, Python immediately exits the try block and jumps to the appropriate except block.

   - in the above code, we attempt to take user input for num1 (numerator) and num2 (denominator). We perform the division operation num1 / num2 inside the try block.

Except Block (except): 
- If an exception occurs in the corresponding try block, Python looks for a matching except block to handle the specific exception type. You can specify the type of exception to catch (e.g., ZeroDivisionError, ValueError) or catch all exceptions using except Exception.

   - (refer code) If the user enters 0 as the denominator (num2), a ZeroDivisionError will occur.
   - The except ZeroDivisionError block catches this specific exception and prints an error message.

   - If the user enters a non-integer value for num1 or num2, a ValueError will occur.
   - The except ValueError block catches this specific exception and prints an error message.

Finally Block (finally): 
- This block is optional and is used to execute cleanup code that should be run regardless of whether an exception occurred or not. It runs whether an exception occurred or not and is generally used to release external resources (like closing files or releasing database connections).

   - (Refer code)This block is always executed after the try and except blocks, regardless of whether an exception occurred or not.
   - Here, it prints a message indicating that the execution has completed and could potentially close any resources (in this case, it's just a print statement).

Output:
         # If the user enters 0 as num2, the output will be:

         Enter numerator: 10
         Enter denominator: 0
         Error: Division by zero is not allowed.
         Execution completed. Closing resources if necessary.

         # If the user enters a non-integer value for either num1 or num2, the output will be:

         Enter numerator: abc
         Error: Please enter valid integers.
         Execution completed. Closing resources if necessary.

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

Answer:
1. Modules:
- Modules in Python are files containing Python code, typically with functions, classes, and variables defined. Each Python script (.py file) is a module, and you can import these modules into other Python scripts to reuse their functionality.

Example: 

         # se_module.py
         def greet(name):
            print(f"Hello, {name}!")

         def add_numbers(a, b):
            return a + b

Importing 'se_module'  

         # main.py
         import se_module

         se_module.greet("Vijo")  # Output: Hello, Vijo!
         result = se_module.add_numbers(5, 3)
         print(result)  # Output: 8

2. Packages:
- Packages are namespaces containing multiple modules grouped together. They are directories that include a special __init__.py file to indicate that the directory should be treated as a package by Python.

Example: 

         se_package/
         ├── __init__.py
         ├── module1.py
         └── module2.py

Inside module1.py, you have:

         # module1.py
         def hello():
            print("Hello from module1!")

Importing 'module1' from 'se_package' in another script:

         # main.py
         from se_package import module1

         module1.hello()  # Output: Hello from module1!

Example: The 'math' module
The math module in Python provides access to mathematical functions. 

         # Using the math module
         import math

         # Example 1: Using math functions
         print(math.sqrt(25))   # Output: 5.0 (square root)
         print(math.pow(2, 3))  # Output: 8.0 (2 raised to the power of 3)

         # Example 2: Using math constants
         print(math.pi)         # Output: 3.141592653589793 (value of pi)
         print(math.e)          # Output: 2.718281828459045 (value of Euler's number)

         # Example 3: Using trigonometric functions
         print(math.sin(math.radians(90)))  # Output: 1.0 (sine of 90 degrees, converted to radians)


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

Answer:

In Python, you can read from and write to files using built-in functions like open(). 

1. Reading from a File
- To read from a file, you can use the open() function with the mode 'r' (read mode). 

Example: 

         # Script to read from a file and print its content to the console

         file_path = 'Vijo.txt'  # Path to the file you want to read

         try:
            with open(file_path, 'r') as file:
               content = file.read()
               print(content)
         except FileNotFoundError:
            print(f"The file {file_path} does not exist.")
         except Exception as e:
            print(f"An error occurred: {e}")

- The 'o'pen(file_path, 'r')' statement opens the file in read mode.
- The 'with' statement ensures that the file is properly closed after its suite finishes.
- The 'file.read()' method reads the entire content of the file.
- If the file does not exist, a 'FileNotFoundError' is caught and handled.

2. Writing to a File
- To write to a file, you can use the open() function with the mode 'w' (write mode) or 'a' (append mode). 
Example:

         # Script to write a list of strings to a file

         file_path = 'output.txt'  # Path to the file you want to write to
         lines_to_write = ["Hello, World!", "This is a test.", "Writing to a file in Python is easy!"]

         try:
            with open(file_path, 'w') as file:
               for line in lines_to_write:
                     file.write(line + '\n')
            print(f"Successfully wrote to {file_path}")
         except Exception as e:
            print(f"An error occurred: {e}")

- The 'open(file_path, 'w')' statement opens the file in write mode. If the file already exists, it will be overwritten. If it doesn't exist, a new file will be created.
- The 'with' statement ensures that the file is properly closed after its suite finishes.
- The 'file.write(line + '\n')' method writes each line to the file, appending a newline character at the end of each string.
- If an error occurs during the writing process, it is caught and handled.

References:
- Gray hat python - python programming for reverse engineers and hackers

- Black hat python - python programming for hackers and pentesters

- Python for cybersecurity offense & defense

- Leaving the rat race - a freelance python developers guide

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


