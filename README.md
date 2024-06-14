
# Monty 🏰

Welcome to the Monty project! This repository contains a simple bytecode interpreter for Monty ByteCodes files. Monty 0.98 is a scripting language that is first compiled into byte codes (just like Python). It relies on a specific stack-based virtual machine.

## Table of Contents

-   [Description](#description)
-   [Tasks](#tasks)
    -   [0. push, pall](#0-push-pall)
    -   [1. pint](#1-pint)
    -   [2. pop](#2-pop)
    -   [3. swap](#3-swap)
    -   [4. add](#4-add)
    -   [5. nop](#5-nop)
    -   [6. sub](#6-sub)
    -   [7. div](#7-div)
    -   [8. mul](#8-mul)
    -   [9. mod](#9-mod)
    -   [10. comments](#10-comments)
    -   [11. pchar](#11-pchar)
    -   [12. pstr](#12-pstr)
    -   [13. rotl](#13-rotl)
    -   [14. rotr](#14-rotr)
    -   [15. stack, queue](#15-stack-queue)
    -   [16. Brainf*ck](#16-brainfck)
    -   [17. Add two digits](#17-add-two-digits)
    -   [18. Multiplication](#18-multiplication)
    -   [19. Multiplication level up](#19-multiplication-level-up)
-   [How to Run](#how-to-run)
-   [Dependencies](#dependencies)
-   [Author](#author)

## Description

This project implements a bytecode interpreter for Monty ByteCodes files. The interpreter reads bytecode files and executes the corresponding commands. It supports various stack operations and allows for extending functionality by adding more bytecode instructions.

## Tasks

### 0. push, pall

🔢 **Task:** Implement the `push` and `pall` opcodes.

-   **push**: Pushes an element to the stack.
    
    -   Usage:  `push <int>`
    -   If  `<int>`  is not provided or not an integer, print an error message and exit with status  `EXIT_FAILURE`.
-   **pall**: Prints all the values on the stack from the top.
    
    -   Usage:  `pall`

### 1. pint

## 📜 **Task:** Implement the `pint` opcode to print the value at the top of the stack.

-   Usage:  `pint`
-   If the stack is empty, print an error message and exit with status  `EXIT_FAILURE`.

### 2. pop

## 🔄 **Task:** Implement the `pop` opcode to remove the top element of the stack.

-   Usage:  `pop`
-   If the stack is empty, print an error message and exit with status  `EXIT_FAILURE`.

### 3. swap

## 🔄 **Task:** Implement the `swap` opcode to swap the top two elements of the stack.

-   Usage:  `swap`
-   If the stack contains less than two elements, print an error message and exit with status  `EXIT_FAILURE`.

### 4. add

## ➕ **Task:** Implement the `add` opcode to add the top two elements of the stack.

-   Usage:  `add`
-   If the stack contains less than two elements, print an error message and exit with status  `EXIT_FAILURE`.

### 5. nop

## 🚫 **Task:** Implement the `nop` opcode that does nothing.

-   Usage:  `nop`

### 6. sub

## ➖ **Task:** Implement the `sub` opcode to subtract the top element of the stack from the second top element.

-   Usage:  `sub`
-   If the stack contains less than two elements, print an error message and exit with status  `EXIT_FAILURE`.

### 7. div

## ➗ **Task:** Implement the `div` opcode to divide the second top element of the stack by the top element.

-   Usage:  `div`
-   If the stack contains less than two elements, print an error message and exit with status  `EXIT_FAILURE`.
-   If the top element is 0, print an error message and exit with status  `EXIT_FAILURE`.

### 8. mul

## ✖️ **Task:** Implement the `mul` opcode to multiply the second top element of the stack with the top element.

-   Usage:  `mul`
-   If the stack contains less than two elements, print an error message and exit with status  `EXIT_FAILURE`.

### 9. mod

## 🔢 **Task:** Implement the `mod` opcode to compute the remainder of the division of the second top element by the top element.

-   Usage:  `mod`
-   If the stack contains less than two elements, print an error message and exit with status  `EXIT_FAILURE`.
-   If the top element is 0, print an error message and exit with status  `EXIT_FAILURE`.

### 10. comments

💬 **Task:** Handle comments in the bytecode files. Lines starting with `#` should be treated as comments.

### 11. pchar

## 🔤 **Task:** Implement the `pchar` opcode to print the char at the top of the stack.

-   Usage:  `pchar`
-   If the value is not in the ASCII table, print an error message and exit with status  `EXIT_FAILURE`.
-   If the stack is empty, print an error message and exit with status  `EXIT_FAILURE`.

### 12. pstr

## 🔤 **Task:** Implement the `pstr` opcode to print the string starting at the top of the stack.

-   Usage:  `pstr`
-   The string stops when the stack is over, the value of the element is 0, or the value is not in the ASCII table.

### 13. rotl

## 🔄 **Task:** Implement the `rotl` opcode to rotate the stack to the top.

-   Usage:  `rotl`

### 14. rotr

## 🔄 **Task:** Implement the `rotr` opcode to rotate the stack to the bottom.

-   Usage:  `rotr`

### 15. stack, queue

## 🔄 **Task:** Implement the `stack` and `queue` opcodes to switch the mode of the data structure.

-   Usage:  `stack`  to switch to stack mode
-   Usage:  `queue`  to switch to queue mode

### 16. Brainf*ck

🧠 **Task:** Write a Brainf*ck interpreter.

### 17. Add two digits

➕ **Task:** Write a Brainf*ck script that adds two digits given by the user.

### 18. Multiplication

✖️ **Task:** Write a Brainf*ck script that multiplies two digits given by the user.

### 19. Multiplication level up

✖️ **Task:** Write a Brainf*ck script that multiplies two digits given by the user and prints the result followed by a new line.

## How to Run

1.  **Clone the repository:**
    
    `git clone https://github.com/Linf0rd/monty.git`
    
    `cd monty` 
    
2.  **Compile the interpreter:**
    
    `gcc -Wall -Werror -Wextra -pedantic *.c -o monty` 
    
3.  **Run the interpreter:**
    
    `./monty <file.m>` 
    

## Dependencies

-   **GCC:**  Ensure you have the GCC compiler installed. You can install it using:
        
    `sudo apt update`
    
    `sudo apt install build-essential` 
    

## Author

👨‍💻 **Linf0rd**