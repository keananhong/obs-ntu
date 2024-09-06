Created: `15-Aug-2024`, `12:40`
Tags: [[MH1812 - Discrete Mathematics]]

# Euclidean Division
$m = qn + r, 0 \leq r \lt n$
- prime numbers are natural numbers that only have 2 divisors, itself and 1

# Modulo n
- for a positive integer n, a and b are congruent modulo if a-b is an integer multiple of n
- if $a\equiv b \pmod n$
	- $a - b = qn$
	- $a = qn + b$
- $-8\equiv 2\equiv 7 \pmod 5$
	- $-8-2=-10$, -10 is a multiple of 5 (-2)
	- $2-7=-5$, -5 is a multiple of 5 (-1)
- $17\equiv 2\equiv 12 \pmod 5$
	- $17-2=15$, 15 is a multiple of 5
	- $2-12=10$, 10 is a multiple of 5
- To find if a number is congruent, start with the number and keep adding n to find other congruent numbers
- Addition modulo
	- a mod n + b mod n $\equiv$ ( a + b ) mod n
	- a mod n $*$ b mod n $\equiv$ ( a $*$ b ) mod n
	- ![[Pasted image 20240815130219.png]]
	- ![[Pasted image 20240815130410.png]]

# Compute $3^{2022} \pmod 5$
$3^1=3\pmod 5$
$3^2 \equiv 4 \pmod 5$ - 
$3^3 \equiv 3^2*3 \equiv 4*3 \equiv 2 \pmod 5$
$3^4 \equiv 3^3*3 \equiv 2*3 \equiv 1 \pmod 5$
Notice that 2022 = $4*505 + 2$
$2022 = 4*505 + 2$
so $3^{2022} \equiv (3^4)^{505} * 3^2$
$\equiv 1^{505} * 3^2$
$\equiv 4$
