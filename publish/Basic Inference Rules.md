Created: `28-Aug-2024`, `16:47`
Tags: [[MH1812 - Discrete Mathematics]]

### Universal Generalization (UG)

**Definition**:  
Universal Generalization is a rule of inference that allows us to infer a universal statement from a particular statement that has been shown to be true for an arbitrary element.

**Key Points**:

- If P(a)P(a)P(a) is true for an arbitrary individual aaa, then ∀x P(x)\forall x \, P(x)∀xP(x) (for all xxx, P(x)P(x)P(x) is true).
- Used when a property can be shown to hold for any element, allowing us to generalize that it holds for all elements.

**Example**:

1. If you can prove that for any number aaa, if a>0a > 0a>0, then a2>0a^2 > 0a2>0,
2. Then, using Universal Generalization, you can conclude that ∀x (x>0→x2>0)\forall x \, (x > 0 \rightarrow x^2 > 0)∀x(x>0→x2>0).

---

### Universal Instantiation (UI)

**Definition**:  
Universal Instantiation is a rule of inference that allows us to infer a specific instance from a universal statement.

**Key Points**:

- If ∀x P(x)\forall x \, P(x)∀xP(x) is true, then P(a)P(a)P(a) is true for any specific individual aaa.
- It is used to apply a universal statement to a particular case.

**Example**:

1. Given the statement ∀x (x2≥0)\forall x \, (x^2 \geq 0)∀x(x2≥0),
2. We can apply Universal Instantiation to conclude that (52≥0)(5^2 \geq 0)(52≥0) is true for the specific instance x=5x = 5x=5.

---

### Existential Generalization (EG)

**Definition**:  
Existential Generalization is a rule of inference that allows us to infer the existence of at least one element that satisfies a condition, based on a particular instance.

**Key Points**:

- If P(a)P(a)P(a) is true for some specific aaa, then ∃x P(x)\exists x \, P(x)∃xP(x) (there exists at least one xxx for which P(x)P(x)P(x) is true).
- It is used to generalize from a specific instance to an existential statement.

**Example**:

1. If we know that P(3)P(3)P(3) is true (for example, "3 is an odd number"),
2. Then we can use Existential Generalization to conclude that ∃x P(x)\exists x \, P(x)∃xP(x) (there exists an xxx such that xxx is an odd number).

---

### Existential Instantiation (EI)

**Definition**:  
Existential Instantiation is a rule of inference that allows us to infer a specific instance from an existential statement.

**Key Points**:

- If ∃x P(x)\exists x \, P(x)∃xP(x) is true, then there exists some specific individual ccc such that P(c)P(c)P(c) is true.
- It is used to move from a statement about the existence of something to a statement about a specific instance.

**Example**:

1. Given ∃x (x>0)\exists x \, (x > 0)∃x(x>0) (there exists some xxx such that x>0x > 0x>0),
2. We can apply Existential Instantiation to say that there is a specific number, say ccc, for which c>0c > 0c>0.