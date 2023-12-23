# Chapter 2.1: Quantifiers

Introducing words such as "any," "all," and "some," brings more complexity into determining the truth of sentences. Page 45

Special notations: Page 45

\\( P\(x\) \\) asserts that \\( x \\) has property \\( P \\).

Universal quantifier: Operation represented by \\( \forall \\). 
For all variable, variable holds property \\( P \\). Example, \\( \forall x P\(x\) \\).

Existential quantifier: Operation represented by \\( \exists \\). 
For some variable, variable holds property \\( p \\). Example, \\( \exists x P\(x\) \\).

Horizontal lines in proofs mean "Hence," or "Therefore." Page 46

Notation layout: Page 47

Individual variables: \\( \{x_1, x_2, ..., x_n, ... \} \\)

Individual constants: \\( \{a_1, b_1, ..., a_2, b_2, ... a_n, b_n, ..., z_n \} \\)

Predicate letters: \\( A^n_k \\) for \\( \{n, k\} > 0 \\)

Function letters: \\( f^n_k \\) for \\( \{n, k\} > 0 \\)

\\( n \\) for both predicate and function letters is the number of arguments,
and \\( k \\) for both is an indexing number to distinguish
predicates and functions with the same number of arguments.

Terms: Page 47

1. Variables and individual constants are terms.

2. If \\( f^n_k \\) is a function letter and \\( \{t_1, t_2, ..., t_n\} \\) are terms,
then \\( f^n_k\(t_1, t_2, ..., t_n\) \\) is a term.

3. An expression is a term iff it can be shown to be a term based on conditions 1 and 2.

Atomic formulas: If \\( A^n_k \\) is a predicate letter and \( \{t_1, t_2, ..., t_n\} \\) are terms,
then \\( A^n_k\(t_1, t_2, ..., t_n\) \\) is an atomic formula. Page 47

Wfs of quantification theory: Page 47

1. Every atomic formula is a wf.

2. If \\( B \\) and \\( C \\) are wfs, and \\( y \\) is a variable, 
then \\( \neg B \\), \\(B \Rightarrow C \\) and \\( \(\forall y\) B \\) are wfs.

3. An expression is a wf iff it is determined to be a wf by the above two conditions.

Scope: For \\( \(\forall y\) B \\), \\( B \\) is the scope of the quantifier \\( \forall y \\).
"Notice that \\( B \\) need not contain the variable \\( y \\). In that case, we understand \\( \(\forall y\) B \\)
to mean the same thing as \\( B \\)." Page 48

"It was unnecessary for us to use the symbol \\( \exists \\) as a primitive symbol
because we can define existential quantification..." \\( \(\(\exists x\)B\) = \neg\(\(\forall x\)\(\neg B\)\) \\) Page 48

Bound variable: A variable \\( x \\) is bound in wf \\( B \\) if it is in the universal or existential quantifiers,
or it lies within the scope of the quantifier variable. Page 49

Free variable: A variable \\( x \\) is free in wf \\( B \\) if it is not bound. Page 49

Make sure to check out the examples on page 49 in depth. They look interesting

Free (bound) variable: A variable in wf \\( B \\) that has a free (bound) occurrence in \\( B \\). "Thus, a variable may be 
both free and bound in the same wf..." Page 50

Variables \\( x_{i_1}, ..., x_{i_k} \\) are marked as free variables in a wf \\( B \\) by writing \\( B \\)
as \\( B \(x_{i_1}, ..., x_{i_k}\) \\). Page 50

\\( t \\) is free for \\( x_i \\) in \\( B \\) if no free occurrence of \\( x_i \\) in \\( B \\)
is in the scope of any quantifier. Page 50

