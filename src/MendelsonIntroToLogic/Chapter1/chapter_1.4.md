# Chapter 1.4: An Axiom System for the Propositional Calculus

### GENERAL FORMAL THEORY DEFINITION: Page 27

Expression (noun): A finite sequence of the symbols of a formal theory.

Well-formed formulas (wfs): Some subset of the expressions of a formal theory. There is usually an effective procedure to
determine whether a given expression is a wf.

Axioms: Some set of the wfs of a formal theory. 

Axiomatic formal theory: If one can effectively decide if a given wf is an axiom.

Rules of inference: A finite set of relations among wfs that, for some wf \\( B \\) 
and another set of wfs \\( C_j \ | \ j > 0 \\), 
you can decide if the sets \\( C_j \\) is in relation to some Rule of Inference \\( R \\).

Following from (verb): If \\( B \\), with the above declarations,
is in relation to \\( C_j \\) as a result of \\( R \\). We say "\\( B \\) follows
from \\( C_j \\) by virtue of \\( R \\)."

Direct consequence (noun): If \\( B \\), with the above declarations, 
is in relation to \\( C_j \\) as a result of \\( R \\). We say
"\\( B \\) is a direct consequence of \\( C_j \\) by virtue of \\( R \\)."
Noun form of following from.

A formal theory \\( F \\) is defined when the following conditions are satisfied.

1. A countable set of symbols is given for \\( F \\).

2. There exist well-formed formulas based on the above set of symbols.

3. There exist axioms based on the above set of wfs.

4. There exist rules of inference from some wfs to other wfs.

Proof in \\( F \\): A sequence of wfs that, for each step in the sequence,
the step is either an axiom of a formal theory \\( F \\) or 
a direct consequence of some of the preceding wfs by virtue of some inference rule. Page 27

Theorem of \\( F \\): A wf \\( B \\) that is the last step of a proof. 
We say this is a "Proof of \\( B \\) in \\( F \\)." Page 27

Decidable theory: A theory for which you can effectively determine if there is proof. Page 28

Undecidable theory: A theory for which you cannot effectively determine if there is a proof. Page 28

"From an intuitive standpoint, a decidable theory is one for which a machine
can be devised to test wfs for theoremhood, whereas, for an undecidable
theory, ingenuity is required to determine whether wfs are theorems." Page 28

Consequence (noun) in \\( F \\): A wf of a formal theory \\( F \\) is a consequence of a set \\( \Gamma \\) of wfs if for 
a sequence of wfs, \\( B_1, ..., B_k \\), each \\( B_i \ | \ (i > 0) \\) is an axiom or
a consequence of some rule of inference on the preceding wfs in the sequence. Page 28

Deduction of \\( B \\) from \\( \Gamma \\):
Operation represented by \\( \vdash \\). \\( \Gamma \vdash C \\). Read as "\\( C \\) is a consequence of \\( \Gamma \\)."
The above sequence performed for \\( C \\), where \\( C \\) is \\( B_k \\). Page 28

Hypotheses/Premisses of a proof: Elements of \\( \Gamma \\) in the above definition. Page 28

"If \\( \Gamma \\) is the empty set \\( \emptyset \\), then \\( \emptyset \vdash C \\) 
if and only if \\( C \\) is a theorem. It is
customary to omit the sign “\\( \emptyset \\)” and simply write \\( \vdash C \\). Thus, \\( \vdash C \\) is another way
of asserting that \\( C \\) is a theorem." Page 28

Properties of consequence:

"If \\( \Gamma \subseteq \Delta \\) and \\( \Gamma \vdash C \\), then \\(\Delta \vdash C \\).

\\( \Gamma \vdash C \\) iff there is a finite subset \\( \Delta \\) of \\( \Gamma \\) such that \\( \Delta \vdash C \\).

If \\( \Delta \vdash C \\), and for each \\( B \\) in \\( \Delta \\), \\( \Gamma \vdash B \\), then \\( \Gamma \vdash C \\)."
Page 28

### FORMAL THEORY DEFINITION FOR THE PROPOSITIONAL CALCULUS (L): Page 28

1. Symbols = {\\( \neg, \Rightarrow, \(, \), \{A_1, ..., A_i | i > 0\}\\)}. 
The primitive connectives are \\( \neg, \Rightarrow \\). 
The letters \\( A_i \\) are statement letters.

2. All statement letters are the well formed forms. Statement forms connected by the primitive connectives are also
statement forms.

3. For statement forms \\( B, \ C \\) and \\( D \\) of L, the following are L's axioms.

    A1: \\(B \Rightarrow \(C \Rightarrow B\) \\)

    A2: \\( \(B \Rightarrow \(C \Rightarrow D)) \Rightarrow \(B \Rightarrow C\) \Rightarrow \(B \Rightarrow D\)\\)

    A3: \\( \(\(\neg C\) \Rightarrow \neg B \) \Rightarrow \(\(\neg C) \Rightarrow B\) \Rightarrow C \\)

4. The only inference rule of L is modus ponens (MP).

Modus Ponens: Operation represented by MP. 
For statement forms \\( B \\) and \\( C \\), \\( B \vdash C \\) and \\( B \Rightarrow C \vdash C \\). Page 29

L is an axiomatic theory because we can tell whether a given wf is of the form A1, A2 or A3. Page 29

Connectives introduced by definition.

D1: \\(B \land C = \neg\(B \Rightarrow \neg C\) \\)

D2: \\( B \lor C = \neg B \Rightarrow C \\)

D3: \\( B \Leftrightarrow C = \(B \Rightarrow C\) \land \(C \Rightarrow B\) \\). Page 29

# Lemma 1.8: Page 29

\\( \vdash_L \Rightarrow B \\)

## Proposition 1.9 (DEDUCTION THEOREM): Page 30

If Γ is a set of wfs and \\( B \\) and \\( C \\) are wfs, and \\( \Gamma \\), \\( B \vdash C \\), 
\\( \Gamma \vdash B \Rightarrow C \\).
In particular, if \\( B \vdash C \\), then \\( \vdash_B \Rightarrow C \\).

# Corollary 1.10: Page 31

If \\( B \Rightarrow C \\) and \\( C \Rightarrow D \\), then \\( D \vdash B \\Rightarrow D \\) and

If \\( B \Rightarrow \(C \Rightarrow D \) \\), then \\( C \vdash B \Rightarrow D \\).

# Lemma 1.11: Page 31

For any wfs \\( B \\) and \\( C \\), the following are theorems of L.

a. \\( \neg \neg B \Rightarrow B \\)

b. \\( B \Rightarrow \neg \neg B \\)

c. \\( \neg B \Rightarrow \(B \Rightarrow C\) \\)

d. \( \(\neg C \Rightarrow \neg B \) \Rightarrow \(B \Rightarrow C\) \\)

e. \\( \(B \Rightarrow C \) \Rightarrow \(\neg C \Rightarrow \neg B\) \\)

f. \\( B \Rightarrow \( \neg C \Rightarrow \neg \(B \Rightarrow C\)\) \\)

g. \\( \(B \Rightarrow C\) \Rightarrow \(\( \neg B \Rightarrow C\) \Rightarrow C\) \\)

# Proposition 1.12: Page 34

Every theorem of L is a tautology.

# Lemma 1.13: Page 34

Refer to the book. I have no clue what this is even saying man FIXME!!!

# Proposition 1.14: Page 35

If a wf of L is a tautology, then it is a theorem of L.

# Corollary 1.15: Page 35

If \\( C \\) is an expression involving the signs \\(\neg, \ \Rightarrow, \ \land , \ \lor \\) and \\( \Leftrightarrow \\) 
that is an abbreviation for a wf \\( B \\) of L,
then \\( C \\) is a tautology iff \\( B \\) is a theorem of L.

# Corollary 1.16

L is consistent, as in, there is no wf \\( B \\) such that both \\( B \\) and \\( \neg B \\) are theorems of L.



