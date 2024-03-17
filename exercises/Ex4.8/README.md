Validity, Satisfiablity, and Unsatifiability
=============================================
This folder contains the proofs of validity, satifiability and unsatisfiablity for dL formula in *Exercise 4.8* of the CPS book. Given a dL formula `P`, we encoded the following in the model.
- If the formula `P` is valid, we prove `P` itself
- If the formula `P` is satisifiable (but not valid), we find two conditions `Q1` and `Q2` and prove that `(Q1 => P) & (Q2 => !P)`. In the case where Q2 is the negation of Q1, we prove `Q1 <=> P`.
- If the formula `P` is unsatisfiable, we prove `!P`.

Automatic vs Interactive
========================
- Most of the proof can be handled by *auto* tactic. Whenever possible, we also provide an *interactive* tactic using basic dL proof rules as they also *explain* the meaning of the formulae and why they are valid/satisfiable/unsatisfiable.
