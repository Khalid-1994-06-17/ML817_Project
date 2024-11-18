# ML817_Project

## Installation Guide

### Prerequisites
- **Python Version**: Ensure you have Python 3.8 or later installed on your system.
- **Pip**: Make sure `pip` (Python's package manager) is updated to the latest version:
  ```bash
  python -m pip install --upgrade pip

## Step 1: Install Standard and Required Libraries
The following libraries are used in this project:

- **Standard Libraries:** Pre-installed with Python, no additional installation required:
numpy, datetime, time, random, collections
- **Required Libraries:** Install these using the following commands.

- **For Intel Chip (macOS or Windows/Linux):**
Run this command in a terminal:

  ```bash
  pip install autograd numpy capytaine matplotlib scipy wecopttool joblib torch

- **For Apple Silicon (macOS with M1/M2 chip):**
Ensure you're using a version of Python and pip compatible with Apple Silicon.
Install most libraries normally:
  ```bash
  pip install autograd numpy matplotlib scipy wecopttool joblib torch

Special Case: `capytaine`
Due to Apple Silicon's architecture, you might need to install capytaine with the `--no-binary` flag:
  
  ```bash
  pip install capytaine --no-binary capytaine

## Step 2: Verify Installation
Run the following command to verify all libraries are installed correctly:

  ```bash
  python -c "import numpy, capytaine, matplotlib, scipy, wecopttool, joblib, torch; print('All libraries installed successfully!')"

- **Additional Notes**
If you encounter issues with capytaine, ensure that you have the necessary C compilers installed on your system. For macOS, you can use:

  ```bash
  xcode-select --install

For troubleshooting torch on Apple Silicon, ensure you're using the appropriate version:

  ```bash
  pip install torch --index-url https://download.pytorch.org/whl/torch_stable.html
