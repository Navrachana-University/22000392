[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/bPoO8GTw)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=19520624&assignment_repo_type=AssignmentRepo)


**A brief descritption of my project:**
This project is a minimalist compiler and interpreter for a custom programming language where all keywords are written in reverse—for example, print becomes tnirp, if becomes fi, and else becomes esle. The language supports basic arithmetic operations (+, -, *, /), variable assignments, conditional statements (nested included), and output printing, effectively functioning as a simple calculator. The compiler performs lexical analysis and parsing, converting the reversed source code into Three Address Code (TAC), which serves as an intermediate representation. An interpreter then processes the TAC to execute the program logic and produce results. This project demonstrates key concepts in compiler construction, including syntax parsing, intermediate code generation, and interpretation, with a creative twist in language design.


Name: **Kirtan Visnagara**
Enrollment ID: **22000392**




# Step 1: Install dependencies (optional, uncomment if needed)
# echo "Installing Flex and Bison..."
# sudo apt-get install -y flex bison

# Step 2: Compile the compiler
flex lex.l
bison -d parser.y
gcc lex.yy.c parser.tab.c -o compiler

# Step 3: Run the compiler on input.txt
compiler input.txt output.txt

# Step 4: Compile the interpreter
gcc interpreter.c -o interpreter

# Step 5: Run the interpreter
interpreter
