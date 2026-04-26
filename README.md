# CVM — Custom Virtual Machine

A lightweight, custom virtual machine and scripting runtime written in C++. CVM interprets `.cvm` scripts through its own instruction set, providing a minimal and self-contained execution environment.

---

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Building from Source](#building-from-source)
  - [Running the VM](#running-the-vm)
- [Usage](#usage)
- [Writing CVM Scripts](#writing-cvm-scripts)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

CVM is a custom virtual machine built in C++ that executes programs written in its own `.cvm` scripting format. The project is designed to explore low-level VM internals, including instruction dispatch, memory management, and runtime execution — all within a clean, portable C++ codebase.

---

## Project Structure

```
CVM/
├── include/          # Header files and public API declarations
├── src/              # Core VM source files (lexer, parser, executor)
├── test.cvm          # Sample script demonstrating the CVM language
├── cvm.exe           # Pre-built Windows executable
└── README.md
```

---

## Getting Started

### Prerequisites

- A C++17-compatible compiler (GCC, Clang, or MSVC)
- Make or any standard C++ build system

### Building from Source

Clone the repository:

```bash
git clone https://github.com/Tanishq96sage/CVM-.git
cd CVM-
```

Compile with g++:

```bash
g++ -std=c++17 -Iinclude src/*.cpp -o cvm
```

Or with MSVC (Windows):

```bash
cl /std:c++17 /I include src\*.cpp /Fe:cvm.exe
```

### Running the VM

On Linux or macOS (after building):

```bash
./cvm test.cvm
```

On Windows using the pre-built binary:

```cmd
cvm.exe test.cvm
```

---

## Usage

```
cvm <script.cvm>
```

| Argument      | Description                        |
|---------------|------------------------------------|
| `script.cvm`  | Path to the CVM script to execute  |

---

## Writing CVM Scripts

CVM scripts use the `.cvm` file extension. Refer to `test.cvm` in the root of the repository for a working example of the script syntax and supported operations.

```cvm
; Example CVM script
; (Refer to test.cvm for full syntax details)
```

---

## Contributing

Contributions are welcome. To contribute:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a pull request.

Please ensure your code follows the existing style and compiles without warnings.

---

## License

This project does not currently specify a license. All rights are reserved by the author unless otherwise stated. Contact the repository owner for usage permissions.

---

*Built with C++ by [Tanishq96sage](https://github.com/Tanishq96sage)*
