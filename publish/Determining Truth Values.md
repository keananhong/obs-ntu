Created: `27-Aug-2024`, `22:36`
Tags: [[MH1812 - Discrete Mathematics]], [[Quantifiers]]

# Via Exhaustion
Let D = ${5,6,7,8,9}$
Is $\exists x \in D, x^2 = x$ True or Flase?
- by manual calculation of 5,6,7,8,9 none of them fulfill this criteria and thus it is false
- good for small domains that arent infinite
-  bro made a truth table ;-;![[Pasted image 20240827223912.png]]

# Method of Case
- find one example where it is true
- can also find counterexample to disprove universal quantification
- only works for proving $\exists$ exsitential quant
	- doesnt work for $\forall$ unless counterexample
	- doesnt work as a counterexample for $\exists$ 
	- since you have to check everything
- Might be hard to find case if it does exist

### **Method of Case: Example**
Let $\mathbb{Z}$ denote all integers
is $\exists x \in \mathbb{Z}, x^2 =x$ true or false?
x=0 or x=1!!!!! it is true asf

### **Method of Case: Counterexample**
Let $\mathbb{R}$ denote all reals
is $\forall x \in \mathbb{R}, x^2>x$ true or false?
x=0.3 is a counterexample. FALSE


# Method of Logiucal Derivation
Consider a domain X with n members
Is $\exists x \in X, (P(x) \lor Q(x)) \equiv (\exists x \in X, P(x)) \lor (\exists x \in X, Q(x))$
Start on LHS
![[Pasted image 20240827225029.png]]
1. expand
2. shift that shit around to group by p and q (since now they are just T/F OR T/F)
3. contract it back