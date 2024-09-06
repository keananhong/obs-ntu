Created: `27-Aug-2024`, `10:01`
Tags: [[SC1005 - Digital Logic]]

# multiplication
![[Pasted image 20240827100255.png]]
- all 4 bits on top times each digit on the bottom, starting from the rightmost one
- shift the numbers left as you proceed
- finally add them all up 

# signed multiplication
- if positive, just do multiplication as per usual
- if negative, then
	- treat the negative MSB bit as a separate number
		- -3  = 1000 + 0101 (-8 + 5)
	- ![[Pasted image 20240827102338.png]]
	- when you multiply 2 numbers of r bits each, the answer will not be more than 8 bits

# Division
![[Pasted image 20240827102556.png]]
- if signed
	- convert the siugn numbers to unsign, divide them as per usual, then convert the result using the appropriate sign representation