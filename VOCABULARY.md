# Vocabulary Alerts

## Runtime in Google Collab
<a name="runtime"></a> 
A **runtime** is the period when a program is actively executing. In environments like Google Colab, the runtime can disconnect after inactivity or due to resource allocation policies, leading to loss of temporary data.

**Example:**  
When Google Colab disconnects, all uploaded data and installed libraries are lost, requiring a fresh setup.

---

## To execute a script
<a name="execute"></a> 
To **execute a script** means to run a Python file in an environment where the code is interpreted and performed by the system.

**Example:**  
Running `python script.py` in the terminal executes `script.py`.

---

## Dependencies in Python
<a name="dependencies"></a> 
**Dependencies** refer to external libraries or modules that a Python project requires to function properly. These are usually installed using package managers like `pip`.

**Example:**  
If a project requires `numpy` for numerical computations, install it using:

```bash
pip install numpy
```

---

## Virtual Environmets
<a name="virtualenvironments"></a> 
A **virtual environment** is a Python environment where the Python interpreter, libraries, and scripts installed into it are isolated from those installed in other virtual environments while still having access to any libraries installed at a system level.

**Example:** 
Sometimes you will need different versions of the libraries and creation of venv will be important to not have conflucts between them.

---

## Standard Library 'venv'
<a name="venv"></a> 
The **venv** module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. A virtual environment is created on top of an existing Python installation, known as the virtual environment’s “base” Python, and may optionally be isolated from the packages in the base environment, so only those explicitly installed in the virtual environment are available. 

**Example**
Creating a virtual environment:

```bash
python -m venv my_env
```

---

## Source the virtual enviromet
<a name="source"></a> 
To **source a virtual environment** means to activate it so that all installed dependencies are used from that environment instead of the system-wide Python installation.

**Example**
After you created the virtual environment, you need to activate it through: 

```bash
source my_env/bin/activate
```

---

## Poit to a specific path
<a name="point-to-a-specific-path"></a> 
Each virtual environment has its own Python interpreter path, which must be selected in VS Code or any other IDE to ensure the correct environment is used.

**Example**
Selecting the virtual environment interpreter in VS Code:

```bash
my_project/.venv/bin/python
```

