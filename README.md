# **Setting Up `graphics.h` in VSCode**

This guide explains how to set up and use `graphics.h` in Visual Studio Code for graphics programming in C++.

---

## **Prerequisites**
You just need these to get started with graphics:
1. **MinGW** (Installed in `C:/mingw`).
2. **Required Files**:
   - `graphics.h`
   - `winbgim.h`
   - `libbgi.a`
3. **VSCode** with the following extensions installed:
   - Code Runner
   - Exe Runner
   - C/C++ Extension Pack
4. **Cloned Repository**:
   - Contains all the required files inside a folder named `required_files`.

---



## **Folder Structure**

After cloning the repository, the project structure should look like this:

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

> **Note:** The `required_files` folder is temporary and can be deleted after setup.

---

## **Setup Instructions**

1. **Clone the Repository:**
   - Open a terminal and run the following command to clone the repository:
     ```sh
     git clone <repository-url>
     ```
   - Replace `<repository-url>` with the actual URL of the repository.

2. **Prepare MinGW:**
   - If you don’t have **MinGW** installed, follow [this video](#) to install it.
   - Once installed, confirm it’s located at `C:/mingw`.

3. **Copy Graphics Files:**
   - Move `graphics.h` and `winbgim.h` to:
     ```
     C:/mingw/include
     ```
   - Move `libbgi.a` to:
     ```
     C:/mingw/lib
     ```

4. **Configure VSCode:**
   - Open the project folder in VSCode.
   - The `.vscode` folder already includes:
     - `c_cpp_properties.json`: Configures C++ include paths.
     - `tasks.json`: Automates build and execution.

5. **Write Your Code:**
   - Write your C++ programs in the `src` folder located inside the `Home` directory.
   - Compiled executables will be generated in the `build` folder.

6. **Run Your Code:**
   - Use the **Code Runner** extension to compile and execute your programs from VSCode.

---

## **YouTube Tutorial**

For a detailed step-by-step tutorial, watch the YouTube video:  
[**How to Set Up `graphics.h` in VSCode**](#)

