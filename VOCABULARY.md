# Vocabulary Alerts

<a name="runtime"></a> 

## **Runtime in Google Colab**
A **runtime** is the period when a program is actively running. In Google Colab, the runtime can disconnect due to inactivity or system policies. This means temporary data like uploaded files and installed libraries will be lost.

**Example:**  
If Google Colab disconnects, you will need to re-upload your files and reinstall any libraries.

---

<a name="execute"></a> 

## To execute a script
To **execute a script** means to run a Python file so the computer can understand and perform its instructions.

**Example:**  
To run a Python file named `script.py`, type this in the terminal:

```bash
python script.py
```

This line executes the output of code `script.py`.

---

<a name="dependencies"></a> 

## Dependencies in Python
**Dependencies** are external libraries that your Python program needs to work correctly. These libraries are installed using package managers like `pip`.


**Example:**  
If a project requires `numpy` for numerical computations, install it using:

```bash
pip install numpy
```

---

<a name="virtualenvironments"></a>

## Virtual Environmets 
A **virtual environment** is a separate space where Python installs libraries for a specific project. This prevents conflicts between different projects that require different library versions.

**Example:** 
If you need different versions of a library for different projects, creating a virtual environment ensures they don't interfere with each other.

Creating a virtual environment:

```bash
python -m venv my_env
```

P.s. "my_env" ca be renaimed into any desired name for the project

---

<a name="standardlib"></a> 

## Python Standard Library 
The **standard library in Python** is a collection of built-in modules and functions that come pre-installed with Python. It provides essential utilities for tasks such as file handling, math operations, data manipulation, networking, and more, allowing developers to perform common programming tasks without needing to install additional packages.

**Example**
- Math Operations (math module)
- Random Number Generation (random module)
- Working with Dates and Time (datetime module)
- Working with Files (os module)
- Handling JSON Data (json module)
- HTTP Requests (urllib module)
- etc

To use the library, add  it to the top part of your code as:
import math

P.s. math can be changed to ay other module from standard python library

---

<a name="source"></a> 

## Source the virtual enviromet
To **source a virtual environment** means to activate it so that all installed dependencies are used from that environment instead of the system-wide Python installation.

**Example**
After you created the virtual environment, you need to activate it through: 

```bash
source my_env/bin/activate # For macOS/Linux
```

```bash
source my_env\Scripts\activate # For Windows
```

---

<a name="point-to-a-specific-path"></a> 

## Poit to a specific path
In Python, pointing to a specific path means specifying the exact location of a file or directory in the system so that Python can access it.

**Example**

1. **Absolute Path**
An absolute path specifies the full location of a file or folder from the root directory.

```python
#Python
file_path = "/Users/username/Documents/my_file.txt"
with open(file_path, "r") as file:
    content = file.read()
```

2. **Relative Path**
```python
#Python
file_path = "data/my_file.txt"
with open(file_path, "r") as file:
    content = file.read()
```

3. In Terminal
```bash
cd ~/Documents/my_project
```

---

<a name="googlecolab"></a> 

## Google Colab
**Google Colab** is a cloud-based platform that allows users to write and execute Python code in an interactive environment. It provides free access to GPUs and TPUs, making it useful for machine learning and data analysis.

**Example**
Colab is useful for machine learning and data analysis because it runs Jupyter Notebooks in the cloud.

---

<a name="host"></a> 

## To host
**To host** means to provide a server where applications, files, or services can be accessed remotely. This can apply to websites, databases, or cloud-based notebooks.

**Example**
Google Colab hosts Jupyter Notebooks in the cloud, so users don’t need to install Python locally.

---

<a name="jupyter"></a> 

## Jupyter Notebook
A **Jupyter Notebook** is an open-source web application that allows users to create and share documents with live code, equations, visualizations, and text.

**Example**
Jupyter Notebooks are widely used in data science and machine learning for interactive coding and visualization.

---

<a name="locally"></a> 

## To run locally
To **run locally** means to execute a program or script on your own computer instead of using a cloud-based service.

**Example**
Instead of using Google Colab, you can install Jupyter Notebook and run Python scripts locally on your machine.

---

<a name="ipl"></a> 

## Interpreted programming Language
An **interpreted programming language** is a language where code is executed line by line by an interpreter instead of being compiled into machine code beforehand.

**Example**
Python is an interpreted language because it runs code directly without compiling it first.

---

<a name="executecode"></a> 

## To execute code
When code is being **executed**, it means that the instructions written in a program are being processed and carried out by the computer.

**Example**
When you press Run in Google Colab, the code cell is executed, and the results appear below it.

---

<a name="interpreter"></a> 

## Interpreter
When code is executed by an **interpreter**, the interpreter reads and runs the code line by line instead of converting it to machine code first.

**Example**
Python’s interpreter runs code immediately, making it easier to debug compared to compiled languages.

---

<a name="cpl"></a> 

## Compiled programming Language
A **compiled programming language** is one where the code is transformed into machine code before execution. This usually results in faster performance compared to interpreted languages.

**Example**
C and C++ are compiled languages, meaning they require compilation before running the program

---

<a name="machine-readble-instructions"></a> 

## Machine-readable instructions 
A compiled programming language converts source code into **machine-readable instructions** that can be directly executed by the computer’s hardware.

**Example**
When you compile a C++ program, it produces an executable file that runs on your system.

---

<a name="terminal"></a> 

## Terminal / Console
A **terminal or console** is a text-based interface where users can interact with the operating system by entering commands.

**Example**
You can run Python scripts from the terminal by typing python name_of_your_script.py.

---

<a name="var"></a> 

## Variable 
A **variable** is a named storage location in memory that holds a value, which can change during program execution.

**Example**
In Python, you can create a variable like this:

```bash
x=10
```

---

<a name="assignval"></a> 

## To assign the value
To **assign a value** means to store a specific piece of data in a variable.

**Example**
Assigning a value to a variable in Python:

```bash
name = "Alice"
```

---

<a name="datatype"></a> 

## Data type
A **data type** defines the type of value a variable can hold, such as integers, floating-point numbers, strings, or lists.

**Example**
Python supports various data types like int, float, str, and list.

```bash
age = 25  # Integer
grade = 89.5  # Float
name = "Alice"  # String
```

---

<a name="declarevar"></a> 

## To declare a variable
To **declare a variable** means to define it and optionally assign a value to it.

**Example**
In Python, you don’t need to explicitly declare variables, just assign a value:

```bash
message = "Hello, world!"
```

---

<a name="ifstate"></a> 

## If statemets
An **if statement** is a conditional structure that allows execution of a block of code only if a specified condition is true.

**Example**
Checking if a number is positive:

```bash
num = 5
if num > 0:
    print("Positive number")
```

---

<a name="condition"></a> 

## Condition in python
A **condition** in Python is an expression that evaluates to True or False and is used in decision-making structures like if statements.

**Example**
A simple condition in an if statement:

```bash
if x == 10:
    print("x is 10")
```

---

<a name="cases"></a> 

## Case in Python
In Python, a **case** refers to a specific condition being checked within a decision-making structure, such as an if-elif-else statement. It is used to evaluate different possible values of a variable and execute the corresponding block of code.
Cases affect conditions by defining multiple possible outcomes using if-elif-else. Each case represents a possible value or range of values for a variable.

**Example**
Checking multiple conditions using if-elif-else:

```bash
fruit = "apple"
if fruit == "banana":
    print("It’s a banana")
elif fruit == "apple":
    print("It’s an apple")
else:
    print("Unknown fruit")
```
