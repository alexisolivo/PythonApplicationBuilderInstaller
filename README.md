# PythonApplicationBuilderInstaller
A bash script to make a python program executable and create a shortcut in the desktop.
Un script de Bash para crear un ejecutable de Python y crear un enlace en el escritorio.

## Overview

This script installs Python 3 and the PyInstaller package on a Linux-based system, and creates a desktop entry for a program called "program_name".
Requirements

This script requires:

- A Linux-based operating system
- sudo privileges to install packages
- Python 3 already installed

## Usage

To use this script, follow these steps:

- Save the script to a file, e.g. "install_program_name.sh".
- Open a terminal window and navigate to the directory containing the script.
- Make the script executable with the following command: chmod +x install_program_name.sh.
- Run the script with sudo privileges: sudo ./install_program_name.sh.

## Script Details

The script performs the following steps:

- Installs Python 3 and pip3 package manager using the apt package manager.
- Installs the PyInstaller package using pip3.
- Sets the program directory to the current working directory.
- Creates a working directory called ".program_name" in the user's home directory.
- Changes the working directory to the ".program_name" directory.
- Uses PyInstaller to create a standalone executable of the "program_name.py" script located in the program directory.
- Creates a desktop entry file named "program_name.desktop" in the user's local applications directory.
- The desktop entry file specifies the program name, description, command to execute the program, terminal behavior, and icon.

## Note

- The program_name.py file should be in the same directory as this script.
- The desktop entry file created by this script may not appear immediately in the user's applications menu until they log out and back in to their system.
