# Vocabulary Alerts

## runtime
<a name="runtime"></a> 
A **runtime** is the period when a program is actively executing. In environments like Google Colab, the runtime can disconnect after inactivity or due to resource allocation policies, leading to loss of temporary data.

**Example:**  
When Google Colab disconnects, all uploaded data and installed libraries are lost, requiring a fresh setup.

---

## To execute a execute
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
<a name="venv"></a> 
A **virtual environment** is a Python environment where the Python interpreter, libraries, and scripts installed into it are isolated from those installed in other virtual environments while still having access to any libraries installed at a system level.

**Example:** 
Sometimes you will need different versions of the libraries and creation of venv will be important to not have conflucts between them.

Creating a virtual environment:

```bash
python -m venv my_env
```

Activating it:

```bash
source my_env/bin/activate
```