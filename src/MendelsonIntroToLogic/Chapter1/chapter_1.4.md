# Chapter 1.4: An Axiom System for the Propositional Calculus

### GENERAL FORMAL THEORY DEFINITION: Page 27

Expression (noun): A finite sequence of the symbols of a formal theory.

Well-formed formulas (wfs): Some subset of the expressions of a formal theory. There is usually an effective procedure to
determine whether a given expression is a wf.

Axioms: Some set of the wfs of a formal theory. 

Axiomatic formal theory: If one can effectively decide if a given wf is an axiom.

Rules of inference: A finite set of relations among wfs that, for some wf *B* and another set of wfs *C*j s.t. j > 0, 
you can decide if the sets *C*j is in relation to some Rule of Inference *R*.

Following from (verb): If *B*, with the above declarations, is in relation to *C*j as a result of *R*. We say "*B* follows
from *C*j by virtue of *R*."

Direct consequence (noun): If *B*, with the above declarations, is in relation to *C*j as a result of *R*. Noun form of
following from. We say "*B* is a direct consequence of *C*j by virtue of *R*."

A formal theory *F* is defined when the following conditions are satisfied.

1. A countable set of symbols is given for *F*.

2. There exist well-formed formulas based on the above set of symbols.

3. There exist axioms based on the above set of wfs.

4. There exist rules of inference from some wfs to other wfs.

Proof in *F*: A sequence of wfs that, for each step in the sequence, the step is either an axiom of a formal theory *F* or 
a direct consequence of some of the preceding wfs by virtue of some inference rule. Page 27

Theorem of *F*: A wf *B* that is the last step of a proof. We say this is a "Proof of *B* in *F*." Page 27

Decidable theory: A theory for which you can effectively determine if there is proof. Page 28

Undecidable theory: A theory for which you cannot effectively determine if there is a proof. Page 28

"From an intuitive standpoint, a decidable theory is one for which a machine
can be devised to test wfs for theoremhood, whereas, for an undecidable
theory, ingenuity is required to determine whether wfs are theorems." Page 28

Consequence (noun) in *F*: A wf of a formal theory *F* is a consequence of a set Γ of wfs if for 
a sequence of wfs, *B*1, ..., *B*k, each *B*i (i > 0) is an axiom or
 a consequence of some rule of inference on the preceding wfs in the sequence. Page 28

Deduction of *C* from Γ: Operation represented by (⊢). Γ ⊢ *C*. Read as "*C* is a consequence of Γ."
The above sequence performed for *C*, where *C* is *B*k. Page 28

Hypotheses/Premisses of a proof: Elements of Γ in the above definition. Page 28

"If Γ is the empty set ∅, then ∅ ⊢ *C* if and only if *C* is a theorem. It is
customary to omit the sign “∅” and simply write ⊢ *C*. Thus, ⊢ *C* is another way
of asserting that *C* is a theorem." Page 28

Properties of consequence:

"If Γ ⊆ Δ and Γ ⊢ *C*, then Δ ⊢ *C*.

Γ ⊢ *C* if and only if there is a finite subset Δ of Γ such that Δ ⊢ *C*.

If Δ ⊢ *C*, and for each *B* in Δ, Γ ⊢ *B*, then Γ ⊢ *C*." Page 28

### FORMAL THEORY DEFINITION FOR THE PROPOSITIONAL CALCULUS (L): Page 28

1. Symbols = {¬, ⇒, (, ), {*A*1, ..., *A*i | i > 0}}. The primitive connectives are ¬, ⇒. The letters *A*i are 
statement letters.

2. All statement letters are the well formed forms. Statement forms connected by the primitive connectives are also
statement forms.

3. For statement forms *B*, *C* and *D*, of L, the following are L's axioms.
    A1: *B* ⇒ (*C* ⇒ *B*)
    A2: (*B* ⇒ (*C* ⇒ *D*)) ⇒ (*B* ⇒ *C*) ⇒ (*B* ⇒ *D*)
    A3: ((¬*C*) ⇒ ¬*B*) ⇒ ((¬*C*) ⇒ *B*) ⇒ *C*

4. The only inference rule of L is modus ponens (MP).

Modus Ponens: Operation represented by MP. For statement forms *B* and *C*, *B* ⊢ *C* and *B* ⇒ *C* ⊢ *C*. Page 29

L is an axiomatic theory because we can tell whether a given wf is of the form A1, A2 or A3. Page 29

Connectives introduced by definition:
    D1: *B* ∧ *C* = ¬(*B* ⇒ ¬*C*)
    D2: *B* ∨ *C* = ¬*B* ⇒ *C*
    D3: *B* ⇔ *C* = (*B* ⇒ *C*) ∧ (*C* ⇒ *B*). Page 29

# Lemma 1.8: Page 29

⊢L *B* ⇒ *B*

## Proposition 1.9 (DEDUCTION THEOREM): Page 30

If Γ is a set of wfs and *B* and *C* are wfs, and Γ, *B* ⊢ *C*, then Γ ⊢ *B* ⇒ *C*. 
In particular, if *B* ⊢ *C*, then ⊢*B* ⇒ *C*.

# Corollary 1.10: Page 31

If *B* ⇒ *C* and *C* ⇒ *D*, then *D* ⊢ *B* ⇒ *D* and

If *B* ⇒ (*C* ⇒ *D*), then *C* ⊢ *B* ⇒ *D*

# Lemma 1.11: Page 31

For any wfs *B* and *C*, the following are theorems of L.

a. ¬¬*B* ⇒ *B*

b. *B* ⇒ ¬¬*B*

c. ¬*B* ⇒ (*B* ⇒ *C*)

d. (¬*C* ⇒ ¬*B*) ⇒ (*B* ⇒ *C*)

e. (*B* ⇒ *C*) ⇒ (¬*C* ⇒ ¬*B*)

f. *B* ⇒ (¬*C* ⇒ ¬(*B* ⇒ *C*))

g. (*B* ⇒ *C*) ⇒ ((¬*B* ⇒ *C*) ⇒ *C*)

# Proposition 1.12: Page 34

Every theorem of L is a tautology.

# Lemma 1.13: Page 34

Refer to the book. I have no clue what this is even saying man FIXME!!!

# Proposition 1.14: Page 35

If a wf of L is a tautology, then it is a theorem of L.

# Corollary 1.15: Page 35

If *C* is an expression involving the signs ¬, ⇒, ∧, ∨ and ⇔ that is an abbreviation for a wf *B* of L, then *C* is a 
tautology iff *B* is a theorem of L.

# Corollary 1.16

L is consistent, as in, there is no wf *B* such that both *B* and ¬*B* are theorems of L.



