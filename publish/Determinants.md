Created: `10-Sep-2024`, `17:36`
Tags: [[SC1004 - Linear Algebra For Computing]]

# What is a determinant?
- ad-bc
- diagonal - non diagonal

Properties
- determinant of i = 1
- determinant changes sign when two rows are swapped
- ![[Pasted image 20240910174103.png]]
- The determinant is a linear function of each row separately
	- |tA| = t|A|
	- ![[Pasted image 20240910174327.png]]
	- if one row of A is added to one row of A', then the determinants add 
		- when teh other rows dont change
		- ![[Pasted image 20240910182252.png]]
		- ONLY when the other rows dont change
	- if 2 rows are equal, then determinant = 0
		- ![[Pasted image 20240910182328.png]]
	- subtracting a multiple of one row from another means determinant is unchanged
	- ![[Pasted image 20240910184628.png]]
	- any matrix with a row of 0s has a determinant of 0
	- If the matrix is triangular, |A| = product of diagonal
	- If A is singular, then |A| = 0, else its not 0
		- When transforming A to U, U has a 0 row
		- thus its determionant is also 0
		- If A is invertible, U has pivots alongits diagonal
			- non-0 pivots = non-0 determinant
			- |A| = +-|U| = +-(product of pivots)
				- +ve for even number of row exchanges, -ve for odd number of row exchanges (becuase of rule 1)
	- ad-bc
	- |AB|=|A||B|
	- |A^T|=|A|

# Determinants as Area or Volume
- a geometric interpretation of determinants
- for 2x2 matrix A, the area of its parallelogram is |A|
- for 3x3 matrix A, the volume of its parallelopiped is |A|

## Can we transform a 2x2 matrix (a1, a2) into a diagonal matrix without changing its area of the associated parallelogram in |A|?
- can interchange two columns
	- since it does not change the parallelogram
	- |A| is unchanged as the rows are not changed
- Add multiple of one column to another

# Calculate area of parallelogram!
1. translate it so that one of the vertices is at the origin
	1. (-2,-2), (0,3),(4,-1),(6,4)
	2. +2, +2 to all
	3. (0,0), (2,5), (6,1), (8,6)
2. The new parallelogram is determined by the columns 2,5 and 6,1 (if you draw it out)
	1. ![[Pasted image 20240910224225.png]]
3. determinant = abs(2 - 30)
4. area = 28

![[Pasted image 20240910224330.png]]

## Linear transformations on area
2x2 trans matrix:
a = transformation matrix
S = paralleolgram
T(S) = |A| x area of s
3x3 trans matrix:
T(S) = abs(|A|) x volume of s

## general case where none of the vertices are at the origin
- has the form p+s
	- p is vector, s is parallelogram at the origin
	- p is a vector that moves the parallelogram away from the origin
- t(p+s) = t(p) +t(S)
	- area of T(p) + T(S)
	- = area of T, as p only moves S and translation does not affect area
	- = |A| x area of s
	- = |A| x area p+S
- also works for arbitrary shapes, not just parallelogram
- ![[Pasted image 20240910231043.png]]