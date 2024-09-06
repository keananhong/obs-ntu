Created: `27-Aug-2024`, `17:28`
Tags: [[MH1812 - Discrete Mathematics]], [[Quantifiers]]

# True vs false quantifications
- $\forall x \in A,P(D)$ 
	- true when P(x) is true for every x in D
	- false when there is at least one x for which P(x) is false_
	- basically $x_1 \land x_2 \land \dots \land x_n$
- $\exists x \in D, P(x)$ 
	- true when there is at least one x in D for which P(x) is true
	- false otherwise
	- basically $x_1 \lor x_2 \lor \dots \lor x_n$

# negations
![[Pasted image 20240827174000.png]]
- To negate an expression, change the quantifier from $\forall$ and $\exists$ to the other one, and negate $\lnot P(x,y)$    the predicant
- not is applied to the predicant
- $\lnot(\forall x \in D, P(x)\land Q(x))$
	- $\equiv \exists x \in D, \lnot(P(x)\land Q(x))$ (negation of quantification)
	- $\equiv x \in D, (\lnot P(x) \lor \lnot Q(x))$ ([DeMorgan's Law](laws%20of%20logic.md#demorgan%20theorem))
	- 