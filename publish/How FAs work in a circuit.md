Created: `27-Aug-2024`, `09:48`
Tags: [[SC1005 - Digital Logic]]

# Title
![[Pasted image 20240827094856.png]]
- loads from the memory, into the registers, into the FAs, store result into register
1. A registers cleared by signal, to value 0000
2. B registers load X from memory
3. FA performs X+0
4. X+0 stpred in A register
5. B register loads Y
6. X+Y performed ion adder
7. A register loaded with X+Y

# Reduce carry propagation
- carry-look-ahead circuit reduces cprop
- many integrated circuits parallel adders use this
