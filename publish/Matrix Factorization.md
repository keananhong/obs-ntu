Created: `04-Sep-2024`, `08:25`
Tags: [[SC1004 - Linear Algebra For Computing]]

# Used in identifying which features in a face is more important

# LU factorization
for a sequence of eqns Ax=b1, Ax=b2, Ax=bn
The inefficient soln would be to compute A inverse for every eqns
Efficient soln
- $A_{m*n} = L_{m*n} * U_{m*n}$
- assuming A can be reduced to [echelon form](matrix%20notation#row%20echelon%20form) without row interchanges
- L = Unit lower triangular
	- Anything above the main diagonal is 0, but everything below the main diagonal is non-zero
- U=upper triangular
	- echelon form
- Ax=b
- LUx = b
- let y=Ux
- Ly=b (solve for y)
- Ux = y (solve for x)
	- easy to solve these 2 eqns  because theboth of them are triangular

# LU Factorization
- Row reduction of A to U produces L without extra work
	- reduce A to echelon form
	- L produced as a byproduct
- There exists unit lower triangular elementary matrices $E_1 to E_p$ such that $E_p \dots E_1A=U$ (turning A into echelon form)
	- Since each elementary matrix represents an ERO
- A = $(E_p \dots E_1)^{-1}U = LU$
- therefore L=$E_p \dots E_1$
- the same row operations that reduce A to U also reduce L to i
- $E_p \dots E_1 L = I$
- ![[Pasted image 20240904084750.png]]
- For teh L matrix,
- Take teh intermediate results (of which have 0s in place) and divide them by the first number in the column
- ![[Pasted image 20240904085001.png]]
- Can also take the inverse of the Ep to E1 matrices
- ![[Pasted image 20240904085052.png]]
- WHen the assum;ition is not valid, use a permutation matrix to swap rows
- swap of r2 and r3![[Pasted image 20240904085315.png]]
- ![[Pasted image 20240904085349.png]]