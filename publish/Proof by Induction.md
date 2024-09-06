Created: `05-Sep-2024`, `10:15`
Tags: 

### Proof by Induction

Proof by induction is a powerful mathematical technique used to prove statements that are true for all positive integers (or for integers within a certain range). It involves two main steps:

1. **Base Case**: Prove that the statement is true for the first value of the integer (usually n=1n = 1n=1, but it can be any starting point).
    
2. **Inductive Step**: Assume that the statement is true for some arbitrary positive integer n=kn = kn=k (called the **inductive hypothesis**) and then prove that the statement is also true for n=k+1n = k + 1n=k+1.
    

If both of these steps are satisfied, the statement is proven to be true for all n≥1n \geq 1n≥1 (or starting from whichever base case is used).

#### Structure of a Proof by Induction:

- **Step 1: Base Case**  
    Verify that the statement is true for the initial case (often n=1n = 1n=1).
    
- **Step 2: Inductive Hypothesis**  
    Assume that the statement is true for some arbitrary n=kn = kn=k. This assumption is made without proving it directly, and it forms the basis of the next step.
    
- **Step 3: Inductive Step**  
    Use the inductive hypothesis (i.e., assume the statement is true for n=kn = kn=k) to show that it must also be true for n=k+1n = k + 1n=k+1.
    

Once these two steps are completed, the statement is proven for all integers greater than or equal to the base case.

#### Example:

Let's prove that the sum of the first nnn positive integers is given by the formula:

1+2+⋯+n=n(n+1)21 + 2 + \dots + n = \frac{n(n + 1)}{2}1+2+⋯+n=2n(n+1)​

**Step 1: Base Case**  
For n=1n = 1n=1, the sum is 111, and the formula gives:

1(1+1)2=1\frac{1(1 + 1)}{2} = 121(1+1)​=1

So the base case holds.

**Step 2: Inductive Hypothesis**  
Assume that the formula is true for some n=kn = kn=k, meaning:

1+2+⋯+k=k(k+1)21 + 2 + \dots + k = \frac{k(k + 1)}{2}1+2+⋯+k=2k(k+1)​

**Step 3: Inductive Step**  
Now, we need to prove that the formula holds for n=k+1n = k + 1n=k+1. The sum up to k+1k + 1k+1 is:

1+2+⋯+k+(k+1)1 + 2 + \dots + k + (k + 1)1+2+⋯+k+(k+1)

By the inductive hypothesis, the sum 1+2+⋯+k=k(k+1)21 + 2 + \dots + k = \frac{k(k + 1)}{2}1+2+⋯+k=2k(k+1)​, so the total sum becomes:

k(k+1)2+(k+1)\frac{k(k + 1)}{2} + (k + 1)2k(k+1)​+(k+1)

Factor out (k+1)(k + 1)(k+1):

k(k+1)2+2(k+1)2=(k+1)(k+2)2\frac{k(k + 1)}{2} + \frac{2(k + 1)}{2} = \frac{(k + 1)(k + 2)}{2}2k(k+1)​+22(k+1)​=2(k+1)(k+2)​

This matches the form of the formula for n=k+1n = k + 1n=k+1, so the inductive step is proven.

Thus, by the principle of mathematical induction, the formula holds for all positive integers nnn.

---

### Complete (Strong) Induction

**Complete induction** (also known as **strong induction**) is a variation of proof by induction. The difference lies in the inductive step: instead of assuming the statement holds for n=kn = kn=k and proving it for n=k+1n = k + 1n=k+1, you assume the statement holds for **all values** of nnn up to kkk and use that assumption to prove it for n=k+1n = k + 1n=k+1.

This form of induction is useful when the statement for n=k+1n = k + 1n=k+1 depends not just on n=kn = kn=k, but also on other earlier values (e.g., n=k−1,k−2n = k - 1, k - 2n=k−1,k−2, etc.).

#### Structure of a Proof by Complete Induction:

- **Step 1: Base Case**  
    Prove that the statement is true for the first value (say n=1n = 1n=1).
    
- **Step 2: Inductive Hypothesis**  
    Assume the statement is true for all values nnn from 1 to kkk.
    
- **Step 3: Inductive Step**  
    Prove that the statement is true for n=k+1n = k + 1n=k+1, using the assumption that it is true for all previous values n=1,2,…,kn = 1, 2, \dots, kn=1,2,…,k.
    

#### Example:

Prove that any integer n≥2n \geq 2n≥2 can be written as a product of primes.

**Step 1: Base Case**  
For n=2n = 2n=2, the number 2 is a prime, so the statement holds.

**Step 2: Inductive Hypothesis**  
Assume that for all integers nnn such that 2≤n≤k2 \leq n \leq k2≤n≤k, the statement is true, meaning that each of these integers can be written as a product of primes.

**Step 3: Inductive Step**  
Now, consider n=k+1n = k + 1n=k+1. There are two possibilities:

- k+1k + 1k+1 is prime. In this case, it is already a product of primes.
- k+1k + 1k+1 is composite. This means k+1=abk + 1 = abk+1=ab, where aaa and bbb are integers less than k+1k + 1k+1. By the inductive hypothesis, both aaa and bbb can be written as products of primes. Therefore, k+1k + 1k+1 can also be written as a product of primes.

Thus, by complete induction, every integer n≥2n \geq 2n≥2 can be written as a product of primes.

---

### Key Differences Between Induction and Complete Induction:

- **Inductive Step**: In regular induction, you assume the statement holds for n=kn = kn=k to prove it for n=k+1n = k + 1n=k+1. In complete induction, you assume the statement holds for all values n≤kn \leq kn≤k to prove it for n=k+1n = k + 1n=k+1.
- **Use Case**: Complete induction is typically used when proving P(k+1)P(k + 1)P(k+1) depends not only on P(k)P(k)P(k), but also on earlier values P(k−1),P(k−2),…P(k-1), P(k-2), \dotsP(k−1),P(k−2),….