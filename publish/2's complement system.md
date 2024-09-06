Created: `26-Aug-2024`, `09:20`
Tags: [[SC1005 - Digital Logic]]

# 2's complement
- the rightmost bit is 0 for +ve and 0
- rightmost bit is 1 for -ve numbers
- has 1 more negative value than positive value
	- e.g. 4 bits -8:7
- we can use 2's complement to subtract numbers in the same way as addition 
	- same set of hardware can be used to do both addition and subtraction

# Conversion
- +ve numbers are the same as original binary, sign bit=0
- if negative, sign bit = 1
- if 2's com of A = B, then 2's com of B =A
1. invert every bit of binary number
2. add 1 to the number
3. add sign bit of 1

# Shortcut
1. starting from least significant bit, copy the bits if they are 0
2. if its the first 1, copy it
3. invert the remaining bits
![[Pasted image 20240826093115.png]]

# Conversion from 2's com to dec
1. take the 2's com of the binary num
2. copnvert to decimal
3. make it negative if its negative
# Patterns
![[Pasted image 20240826094234.png]] 

![[Pasted image 20240826094259.png]]

# facts
- 2's com of n-bit bin num has n bits
- 2's com of n bit bin num is n+1 bit for the sign bit
- if you want to pad the number
	- negative numbers are padded with 1, while postive numbers are padded wiuth 0
		- 101=1101=11101
		- 010=0010=00010
- 2's comming a number will change it from +ve to -ve and vice versa without changing the magnitude
	- EXCEPT The most negative number because we cant represent the +ve of that number
	- ![[Pasted image 20240826095435.png]]\

# Addition
- make sure the sign bit is aligned, then sum them as usual
- ignore carry out past the sign bit
- pair of numbers are result must have the same number of bits

# Subtraction
- A-B = A + -B
- take 2's complement of B

# Overflow
- when the result of addition or subtraction cannot be represented by the n-bits of the operands.
- can detect when +ve + +ve = -ve and vice versa
- ![[Pasted image 20240826105324.png]]