Enconding generic formulae
==========================
We can use definitions to encode generic formulae, e.g., predicates,
real functions, and hybrid programs.
```
Definitions
  // A generic predicate
  Bool P(Real x);
  // A generic (real) function
  Real F(Real x);
  // A generic hybrid program with condition Q,
  // differential equation D and evolution domain E.
  Bool Q(Real x);
  Real D(Real x);
  Bool E(Real x);
  HP   A ::= {?Q(x);x:=*; {x'=D(x) & E(x)}};
End.
```
In the case of hybrid programs, if we want to treat them as generic
programs, we will avoid expanding its definition (eventhough their
structure will be very generic).

Available Rules
===============
Besides logical rules (from Chapter 6), the following rules are available to
reason about hybrid programmes in Chapter 5.
- Assignments (*assignb*)
- Differential equation solution (with/without domain axiom) (*solve*)
- Tests (*testb*)
- Sequential composition (*composeb*)
- Nondeterministic choice (*choiceb*)
- Loops (*iterateb*)
- Diamonds (*diamondd*)

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
