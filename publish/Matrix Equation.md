Created: `03-Sep-2024`, `18:28`
Tags: [[SC1004 - Linear Algebra For Computing]]

# The Matrix Equation
$Ax=b$
A linear system of equations with many unknowns can be written as simultaneous eqns, and in matrix form:
System Form![[Pasted image 20240903183137.png]] 
Matrix Notation
![[Pasted image 20240903183215.png]]
A is the matrix of scalars, and x is the matrix of unknowns
- In other words, Ax is the linera combination of columns of A using the corresponding entries in x as weights
- Ax=b only has a solution if bn is  a linear combination of the columns of A
- Consistent means does it have a solution or not?![[Pasted image 20240903183701.png]]
	- solve using the [usual method](Linear%20combination%20of%20vectors#Question!)
	- The columns of A (meaning each column) spans a plane through the origin

Theorem
- A is invertible only if there is an EROs that turn it into I. Teh same EROs turn it from I  into A^-1
![[Pasted image 20240904082328.png]]

