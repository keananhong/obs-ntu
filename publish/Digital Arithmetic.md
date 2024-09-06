Created: `20-Aug-2024`, `17:35`
Tags: [[SC1005]]

# here
![[Pasted image 20240820180748.png]]

# Adders
- Half Adder
- ![[Pasted image 20240820200258.png]]
	- but half adder cannot add 3 bits
	- sum is a xor b
	- carry is ab
- Full adder
	- ![[Pasted image 20240820200340.png]]
	- carry input
	- the boolean expression of this table
		- Sum = A xor B xor Cin
		- Cout = A* B + B * Cin +A * Cin
	- full adder circuit![[Pasted image 20240820200635.png]]

# Binary Math
- Full adder can be used to add two binary numbers
- ![[Pasted image 20240826085931.png]]
- 3 inputs: carry from previous sum, top bit and bottom bit
- you will need one full adder per bit in the addition
	- cascaded full adders are known as a ripple addder
	- very fast, and speed of it is limited by propagation delay of FAs (carry rpopagation)
	- ![[Pasted image 20240826090332.png]]
	- full adder on teh right will have the least significant bit, while rightmost is the most significant bit
	- propagation delay is the time it takes for the carry of one FA to reach the next full adder, therefore a number of n bits has n prop delay