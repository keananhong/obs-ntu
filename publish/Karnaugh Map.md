Created: `10-Sep-2024`, `23:34`
Tags: [[SC1005 - Digital Logic]]

# K-map
- need to label squares such that they differ in only one variable
- remember this such that u dont use the same sequebnce as binaries
- SOP
	- circling squares that contain 1 and OR them tgt
- POS 
	- circling squares that contain 0 and AND them tgt
2 input
![[Pasted image 20240910233822.png]]

3 inputs
![[Pasted image 20240910233949.png]]
- 2 vars on left, one var on top

4 input
![[Pasted image 20240910234121.png]]

Be aware of the sequence in the K-map, will make transfers easier
![[Pasted image 20240910234235.png]]

## Obtain Loops
- loop neighbouring 1s
- ![[Pasted image 20240911002734.png]]
- green loop = 2 rows 1 col
	- B does not matter, as it does not affect outcome
	- therefore, A'C'D
- purp loop
	- C does not matter
	- ABD
- red loop
	- C does not matter
	- AB'D'
- blue loop
	- A does not matter
	- B'CD'
- eliminates 1 variable!!

![[Pasted image 20240911003151.png]]
4 loopys
pink loop
- BD
red loop
- A'B'
Blue loop
- A does not matter
- C does not matter
- B'D'

![[Pasted image 20240911003526.png]]
8 loopies

## Rules for simplification
- only loop 1s for SOP
- only loop $2^n$ number of 1s together
- no looping along diabonal
- all 1s must be looped
- use biggest and fewest loops
- a square can be looped more than 1s
- each loop results in a product 
- only loop 0s for POS
	- will give sum term

# Simplification
![[Pasted image 20240911004450.png]]
![[Pasted image 20240911004613.png]]
