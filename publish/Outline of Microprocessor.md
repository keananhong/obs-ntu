Created: `14-Aug-2024`, `21:39`
Tags: [[SC1003 - Computational Thinking]]

# Parts of a microprocessor
- [[Computer organisation]]

# CPU parts
- Control Unit (CU)
	- controls and coordinates overall operation of CPU
	- consists of decoders and logic circuits
	- controls overall of the various units and modules
	- a clock signal ensures that all operations happen at the correct instances and in the proper sequences
- Arithmetic Logic Unit (ALU)
	- performs arithmetic and Boolean logic functions
- Register Array
	- Holds information used by CPU operations
	- small amount of very high speed internal storage used for frequently accessed data like cache?
	- allows the fast storage and retrieval of data
- PC
	- program counter, indicates address of machine instructions in the memory
- IR
	- Instruction Register stores the instruction to be decoded
- CU
	- kontol unit that coordinates operation of the CPU inluding the decoding of the instruction

## DAta address and control signals
- comprises of signaling wires, grouped into 
	- data signals
	- address signals
	- control signals
- these signals help operations by connecting the internal functional units together
- also is extended to the external system bus for other modules like memory and Inputoutpit of the micrtoprocessor

## Different bus types
- Data bus
	- transfers info from one module to another
- Control bus 
	- provides control signals ^ for modules to work together 
	- like determining data flow
	- determines when which device can access the data and address bus
- Address Bus
	- transfers address information of memory i guess?
	- Determines the source and destionation of the data transfer
