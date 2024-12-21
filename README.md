# How-to-Setup-Graphics.h-for-Visual-Studio-Code

This guide provides a step-by-step approach to setting up and using `graphics.h` in Visual Studio Code for graphics programming in C++.

---

## Prerequisites
Ensure you have the following tools and files ready before proceeding:

1. **MinGW** (installed at `C:/mingw`).
   If your preinstalled MinGW fails to work, reinstall it from this [link](https://sourceforge.net/projects/mingw/).
   ![image](https://github.com/user-attachments/assets/7aa0e871-2665-462c-b001-7332d0c28b9f)
   Click the first download link on the home page. Continute the installation procedure, make sure to check mark all the basic setup packages.
3. **Required Files**:
   - `graphics.h`
   - `winbgim.h`
   - `libbgi.a`
4. **VSCode** with these extensions installed:
   - Code Runner
   - Exe Runner
   - C/C++ Extension Pack
5. **Cloned Repository**:
   - Contains all the required files in a folder named `required_files`.

---

## Folder Structure
After cloning the repository, the project directory should look like this:

```
Project Folder
├── .vscode
│   ├── c_cpp_properties.json
│   └── tasks.json
├── Home
│   ├── src (Your source code goes here)
│   └── build (Compiled executables will be here)
├── required_files
│   ├── graphics.h
│   ├── winbgim.h
│   └── libbgi.a
```

> **Note:** The `required_files` folder is only needed during setup and can be removed afterward.

---

## Setup Instructions

### 1. Clone the Repository
Open a terminal and run the following command:

```bash
git clone <repository-url>
```

Replace `<repository-url>` with the actual URL of the repository.

---

### 2. Install MinGW (If Not Installed)
If MinGW is not already installed:

- Follow [this video tutorial](https://www.youtube.com/watch?v=AIX8JSr6MQY) for installation.
- Ensure MinGW is installed at `C:/mingw`.

---

### 3. Copy Required Graphics Files

Move the following files to the specified directories:

- `graphics.h` and `winbgim.h` to:

  ```
  C:/mingw/include
  ```

- `libbgi.a` to:

  ```
  C:/mingw/lib
  ```

---

### 4. Configure VSCode

- Open the project folder in VSCode.
- The `.vscode` folder already contains the necessary configuration files:
  - `c_cpp_properties.json`: Configures C++ include paths.
     Check this file for any yellow underlines, as they may indicate that the file paths need to be updated to match your system. Ensure MinGW is installed in the C: drive (e.g., C:\mingw64). If the issue persists, consider reinstalling MinGW as described earlier.
  - `tasks.json`: Automates build and execution.

---

### 5. Write Your Code

- Create your C++ programs in the `src` folder inside the `Home` directory.
- Compiled executables will be automatically saved in the `build` folder.

---

### 6. Build and Run Your Code

- Use the **Code Runner** extension to compile and execute programs directly within VSCode.
- To build the project:
  - Press `CTRL+SHIFT+B`. This will compile the code and generate executables in the `build` folder.

---

### 7. Run the Executable File

- Use the **Exe Runner** extension to execute the compiled graphics program:
- Look for the "Run Executable" button in the top-right corner of VSCode and click it to run your graphics program.

---

## YouTube Tutorial

For a detailed walkthrough of the setup process, watch the [YouTube tutorial](https://www.youtube.com/watch?v=AIX8JSr6MQY).

---

By following this guide, you’ll have `graphics.h` fully set up in VSCode and ready for your graphics programming projects!

