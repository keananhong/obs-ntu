### From decimal to base x
- divide by x until quotient is 0
- remainders from bottom up is the answer
	- 8/2=4R0
	- 4/2=2R0
	- 2/2=1R0
	- 1/2=0R1
	- answer is 1000
- For decimal points
	- Multiply by x until ans is 0
	- C stands for carry over
		- 0.375x2=0.75C0
		- 0.75x2=0.5C1
		- 0.5x2=0C1\

### Converting between bases of power 2
- First convert to binary
- Group according to how many bits in the power
	- if base 16, group binary into 4 bits, starting from decimal point
	- if base 8, group into 3 bits
	- if base 4, group into 2 bits
- Convert each group into its base x digit
	- 1010 1111
		- 1010 = A
		- 1111 = F
		- ans is AF

[[SC1005 - Digital Logic]]