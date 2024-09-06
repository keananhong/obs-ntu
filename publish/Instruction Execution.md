Created: `14-Aug-2024`, `22:32`
Tags: [[SC1003 - Computational Thinking]]

# Steps of executing instructions
1. when powered up, program instructions is first loaded into default memory locations with data
2. clocking signal is applied to microprocessor
3. When the clock edges rises or falls, CU fetches instructions from the default memory location
4. CU recognises its own instructions and performs them

# Special registers needed
- Program Counter (PC)
	- tells CU where instructions are in memory
- Instruction Register (IR)
	- holds the copy of the instruction to be decoded and executed from the memory
	- instruction gotten using address from PC

![[Pasted image 20240814223734.png]]
