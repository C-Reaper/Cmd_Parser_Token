# Project README

## Overview
The project is a C/C++ parser that demonstrates the use of custom tokenization and parsing rules. The main goal is to parse a string expression, apply transformations based on specific rules, and print the result.

## Features
- Custom keyword recognition
- Operator precedence handling with transformation flags
- String parsing and manipulation

## Project Structure
### Prerequisites
- C/C++ Compiler (GCC, Clang)
- Make utility
- Standard development tools

## Build & Run
To build and run the project on different platforms:

**Linux:**
```bash
make -f Makefile.linux all
./build/Main
```

**Windows:**
```bash
make -f Makefile.windows all
build\Main.exe
```

**Wine (Linux cross-compile for Windows):**
```bash
make -f Makefile.wine all
wine build/Main.exe
```

**WebAssembly (Emscripten):**
```bash
make -f Makefile.web all
wasmtime build/Main.wasm
```

Each makefile provides specific commands for building, cleaning, and debugging the project. The `do` target is provided for a one-stop build and execution process.