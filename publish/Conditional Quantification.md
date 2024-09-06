Created: `27-Aug-2024`, `23:26`
Tags: [[MH1812 - Discrete Mathematics]], [[predicates]]
Previous: [[Determining Truth Values]]

# Example 1
- for any real number X, if x > 1 then x^2 > 1
P(x) = x>1
Q(x) = $X^2 > 1$
For $\forall x \in \mathbb{R}, (P(x) \rightarrow Q(x)$ 

# Example 2
- many statements can be restated as conditional statmenets
- Lions are fierce animals
A is collection of all animals
P(x) denotes x is a lion
Q(x) denotes x is fierce
can be rephrased as if an animal x is a lion then x is fierce
$\forall x \in A, (P(x) \rightarrow Q(x))$
![[Pasted image 20240827233559.png]]

# Negating conditional quantification
- What is $\lnot (\forall x \in X, P(x)\rightarrow Q(x))$
- ![[Pasted image 20240827233710.png]]
- 1. negate quantified statements
	- change forall to exists, lnot the statement inside
	- convert the rightarrow [conversion law](Conditional%20Operators#Conversion%20Theorem)
	- [DeMorgan's Law](laws%20of%20logic.md#demorgan%20theorem) that shit