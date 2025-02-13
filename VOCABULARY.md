# Vocabulary Alerts

<a name="runtime"></a> 
## Runtime in Google Collab
A **runtime** is the period when a program is actively executing. In Google Colab, the runtime can disconnect due to inactivity or system resource policies, leading to the loss of temporary data like uploaded files and installed libraries.

**Example:**  
If Google Colab disconnects, all uploaded files and installed libraries will be lost, requiring you to re-upload and reinstall them.

---

<a name="execute"></a> 
## To execute a script
To **execute a script** means to run a Python file in an environment where the code is interpreted and performed by the system.

**Example:**  
Running:

```bash
python name_of_your_file.py 
```

in the terminal executes the output of code `name_of_your_file.py`.

---

<a name="dependencies"></a> 
## Dependencies in Python
**Dependencies** refer to external libraries or modules that a Python project requires to function properly. These are usually installed using package managers like `pip`.

**Example:**  
If a project requires `numpy` for numerical computations, install it using:

```bash
pip install numpy
```

---

<a name="virtualenvironments"></a>
## Virtual Environmets 
A **virtual environment** is an isolated Python environment where the interpreter, libraries, and scripts are separate from the system-wide installation. This prevents conflicts between different projects that require different library versions.

**Example:** 
If you need different versions of a library for different projects, creating a virtual environment ensures they don't interfere with each other.

---

<a name="venv"></a> 
## Standard Library 'venv'
The **venv** module is used to create lightweight virtual environments. Each virtual environment has its own Python installation and independent package directory. This allows for better project dependency management.

**Example**
Creating a virtual environment:

```bash
python -m venv my_env
```

P.s. "my_env" ca be renaimed into any desired name for the project

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
Each virtual environment has its own Python interpreter path. This path must be selected in IDEs like VS Code to ensure the correct environment is used.

**Example**
Selecting the virtual environment interpreter in VS Code:

```bash
my_project/.venv/bin/python
```

