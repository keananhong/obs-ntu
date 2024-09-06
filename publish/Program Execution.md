Created: `14-Aug-2024`, `22:18`
Tags: [[SC1003 - Computational Thinking]]

# About programs
- programs (instructions) are loaded into the memory in binary with the data
- when loaded, it contains the instructions to be executed, and the data needed bythe instructions

## Program execution
Done in 3 basic steps
1. Fetch instruction from the memory to the CPU
2. Decode the instructions 
3. Execute the decoded instructions

# CPU operation
- Instructions are fetched to the CPU by the control unit
- its then loaded into the memory in binary, just liek the data
	- we dont know which is which but the computer does

# Instructions
- Valid instructions are encoded in specific binary patterns
	- known as instruction set of microprocessor
		- AKA x86, x64, ARM
- CPU recognises its own instructions

# Stored program model
shows how shit from the memory is executed
1. data is moved from memory (RAM) to the CPU registers (control unit's orders)
2. control unit tells ALU to do operation of num1+num2
3. control unit stores the sum inside another register
4. control unit moves the sum from the register into the memory