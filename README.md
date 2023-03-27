Monty Interpreter
Monty is a simple interpreter for a subset of the stack-based programming language Monty. Monty uses a stack to evaluate expressions and has a small number of operations.

Installation
To build the Monty interpreter, clone the repository and compile the source code using gcc:

bash
Copy code
git clone https://github.com/<username>/monty.git
cd monty
gcc -Wall -Werror -Wextra -pedantic *.c -o monty
Usage
The Monty interpreter can be run with a Monty bytecode file:

bash
Copy code
./monty bytecode.m
Supported Operations
The Monty interpreter supports the following operations:

push <int>: Pushes an element to the stack
pall: Prints all the values on the stack
pint: Prints the value at the top of the stack
pop: Removes the top element of the stack
swap: Swaps the top two elements of the stack
add: Adds the top two elements of the stack
nop: Does nothing
sub: Subtracts the top element of the stack from the second top element
div: Divides the second top element of the stack by the top element
mul: Multiplies the second top element of the stack with the top element
mod: Computes the modulus of the second top element of the stack with the top element
pchar: Prints the ASCII character value of the top element of the stack
pstr: Prints the string starting at the top of the stack
rotl: Rotates the stack to the top
rotr: Rotates the stack to the bottom
queue: Sets the format of the stack to a queue
stack: Sets the format of the stack to a stack
Example
Consider the following Monty bytecode file example.m:

perl
Copy code
push 1
push 2
push 3
pall
add
pall
The output of the Monty interpreter when run with this file is:

Copy code
3
2
1
5
2
1
Author:
Maskoli Favour
