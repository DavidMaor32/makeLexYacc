# Compiler Project with Makefile

This project is designed to help you create a compiler using Lex and Yacc with the provided Makefile template. Follow the instructions below to set up and generate your compiler.

## How to Use

1. **Copy Template**
   - Copy the provided Makefile template to the project directory.

2. **Create Lex and Yacc Files**
   - Ensure you have created your Lex (`*.l`) and Yacc (`*.y`) files.

3. **Run Commands in Terminal**

    ```bash
    # Navigate to the project directory
    cd ./myProject
    
    # Generate the compiler
    make
    
    # Compile the source file 'text.t'
    ./myCompiler < text.t
    
    # Clean up generated files
    make clean
    ```

## Example

```bash
# Change working directory to the project
cd ./myProject

# create and write the lex file
nano scanner.l

# create and write the yacc file
nano parser.y

# Generate the compiler
make

# Compile the source file 'text.t'
./myCompiler < text.t

# Delete the compiler, lex.yy.c, and y.tab.c
make clean
