Created: `26-Aug-2024`, `22:39`
Tags: [[SC1004 - Linear Algebra For Computing]]

# Linear combination
Get teh vectors and multiply them by given scalars
$y=c_1v_1 + ... + c_pv_p$


## Question!:
$$a_1=\begin{bmatrix}
1 \\
-2 \\
-5 \\
\end{bmatrix}
, a_2=\begin{bmatrix}
1 \\
5 \\
6 \\
\end{bmatrix},
b=\begin{bmatrix}
7 \\
4 \\
-3 \\
\end{bmatrix}
$$
Determine whether b can be written as a linear combination of $a_1$ and $a_2$
$x_1\overrightarrow a_1 + x_2\overrightarrow a_2 = \overrightarrow b$
$\color{lightblue}\heartsuit$
$x_1\begin{bmatrix}1\\-2\\-5\\\end{bmatrix}+x_2\begin{bmatrix}2\\5\\6\\\end{bmatrix}=\begin{bmatrix}7\\4\\-3\\\end{bmatrix}$

$x_1+2x_2=7$
$-2x_1+5x_2=4$
$-5x_1+6x_2=-3$
now we find the reduced row echelon form
augmented matrix = $\begin{bmatrix}1&2&7\\-2&5&4\\-5&6&-3\\\end{bmatrix}$
after some transformations (not limited to) $r_2 \leftarrow 2r_1+r_2$ and $r_3 \leftarrow 5r_1-r_3$
final form: $$ x= \begin{bmatrix}1&0&3\\0&1&2\\0&0&0\\\end{bmatrix} $$
$x_1=3$ and $x_2=2$
therefore,
$$3\begin{bmatrix}1\\-2\\-5\\\end{bmatrix}+2\begin{bmatrix}2\\5\\6\\\end{bmatrix}=\begin{bmatrix}7\\4\\-3\\\end{bmatrix}$$

![[Pasted image 20240826230838.png]]b (the RHS) can only be expressed as a linear combintaion of vectors if there is at least one solution to the linear system represented buy the augmented matrix
ANd
if b can be represented by a linear combination, then there is at least one solution for the system

# Find solutions
1. First find reduced row echelon form (using simultaneous eqns)
	1. basically make the 0 staircase
2. calculate from bottom up to see if there are soutions for the vars
3. if its impossible, like bottom row is 0 0 3, then there is no soluyton for it