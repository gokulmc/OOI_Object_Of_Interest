Installation steps
If you’ve created a new project folder in VS Code and want to run Python code, here’s a step-by-step checklist of what to do before running any code.

1. Install Python

Make sure Python 3.9+ is installed on your system.
Check version:
->        python --version

2. Create a Virtual Environment (Recommended)

A virtual environment keeps your project’s packages separate from global Python.
->        python -m venv .venv

.venv is the folder name for your environment (common convention).

3. Activate the Virtual Environment
Windows (PowerShell):

->       .\.venv\Scripts\activate

4. Select the Python Interpreter in VS Code
->        Press Ctrl+Shift+P → type Python: Select Interpreter
Choose the interpreter from .venv you just created.

5. Install Required Packages
Use pip install to install all packages your code needs. Example for YOLO + DeepSORT tracking:
->        pip install ultralytics opencv-python deep-sort-realtime
Note: You only install packages once per environment, even if you create multiple files.

6. Optional: Check Installation
->        python -c "import cv2; import ultralytics; import deep_sort_realtime; print('Packages installed correctly')"

7. Run Your Script
Navigate to your project folder in terminal:
->        cd path\to\your\project
eg cd 


8. Run your Python file:
->        python your_script.py

    <!-- Summary
    Install Python

    Create & activate a virtual environment

    Select interpreter in VS Code

    Install required packages via pip

    Run your Python script -->