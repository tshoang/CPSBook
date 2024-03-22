Validity, Satisfiablity, and Unsatifiability
=============================================
This folder contains the proofs of validity, satifiability and unsatisfiablity for dL formula in *Exercise 4.8* of the CPS book. Given a dL formula `P`, we encoded the following in the model.
- If the formula `P` is valid, we prove `P` itself
- If the formula `P` is satisifiable (but not valid), we find two conditions `Q1` and `Q2` and prove that `(Q1 -> P) & (Q2 -> !P)`. In the case where Q2 is the negation of Q1, we prove `Q1 <-> P`.
- If the formula `P` is unsatisfiable, we prove `!P`.

Automatic vs Interactive
========================
Most of the proof can be handled by *auto* tactic. Whenever possible, we also provide an *interactive* tactic using basic dL proof rules as they also *explain* the meaning of the formulae and why they are valid/satisfiable/unsatisfiable.

Checking with KeymaeraX command line
====================================
The *.kyx can be proved by command line with KeymaeraX using the following command
```
java -jar /path/to/keymaerax.jar -prove file.kyx
```
where `/path/to/keymaerax.jar` is the path to the KeymaeraX jar file and `file.kyx` is the name of the input file.

Exploring with KeymaeraX UI
===========================
Launch KeymaeraX UI (default) and create a model and copy the content
of the *.kyx file. Try to follow the steps of the interactive proof to
see their details (or load the proof automatically).

Summary
=======
Here is the summary for the different questions
1. Valid
2. Satisfiable
3. Satisfiable
4. Valid
5. Unsatisfiable
6. Valid
7. Valid
8. Valid
9. Unsatisfiable
10. Valid
11. Valid
12. Valid
13. Unsatifiable
14. Valid
15. Unsatifiable
16. Satisfiable
17. Valid
18. Satisfiable
19. Valid
20. Valid
