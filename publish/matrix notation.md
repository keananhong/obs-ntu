Created: `26-Aug-2024`, `16:58`
Tags: [[SC1004 - Linear Algebra For Computing]]

# Equation can be represented by matrix
- coefficient matrix: just shows teh matrix of coefficients of x and y
- augemneted: shows teh coefficients as well as c
- ![[Pasted image 20240826165908.png]]

# 2 questions about a linear system
	- is it consistent? does at least one solution exist
	- if there is a solution, is there only one
- can answer these by converted augmented matrix row equivalent

## Elementary Row operations
1. multiply a row by a constant
2. interchange two rows
3. add a constant times one row to another
4. ![[Pasted image 20240826211714.png]]
5. 
# Row echelon form
a matrix is in row echelon form if it
- groups all the rows that consist of only 0s at the botton of the matrix
- in any two consecutive non-zero rows, the first element (pivot) of the lower row is to the right of the pivot in the previous row

## Reduced Echelon form
a matrix is in reduced echelon form if it
- is in row echelon form
- in every column with a pivot, the pivot has the value 1 and all other elements IN TEH COLUMN are 0
- guassian eliminiation can be used to convert a matrix into row echelon form through a sequence of EROs
- gauss-jordan elimination is a matrix that is not in reduced row echelon form can be transformed into one throuigh a sequence of EROs![[Pasted image 20240826213200.png]]

# Answering qns with the echelons
![[Pasted image 20240826213749.png]]

![[Pasted image 20240826213808.png]]

# Solutions of linear systems
![[Pasted image 20240826214758.png]]Infinite solutions, as any value of x1 to x6 satisfies this last eqn, and thus infinite number of solutions
- find the reduced row echelon form
- take the leading variable
- solve for leading variables
- give the other variables arbtrary values r s t![[Pasted image 20240826221818.png]]

# Total steps to use row reduction to solve a linear system
1. Write augemneted matrix
2. use row reduction algo to get the row echelon form and if the system has at least one solution, continue
3. get reduced row echelon form
4. write system of eqns corresponding to step 3 matrix
5. rewrite each nonzero eqn from step 4 so that its one leading variable is expressed in terms of any free variables appearing in the eqn