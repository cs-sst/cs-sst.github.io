---
layout: page
title: Implementation
permalink: /faculty/nivelle/implementation/index
---

## Geo III

At this moment, Geo III is an unfinished prover for classical logic 
with partial functions, based on 
[Kleene Logic](https://cs-sst.github.io/faculty/nivelle/publications/index/jlc2014.pdf)
In the current version, only Chapters 4 and 5 have been implemented,
and the transformation from first-order logic to geometric logic
is still 2-valued. 
The goal of Geo III is to eventually implement the complete logic.
I assume that this goal will be reached in the fall of 2018,
because I wanted to work on matching first. 

### Downloading

The latest public version is geo2016C.
It can be downloaded from 
[CASC](http://www.cs.miami.edu/~tptp/CASC/J8/SystemsSources/).
Note that Geo is released under GNU General Public Licence, Version 3.

At CASC J9, there will be a new version. 

### Running Geo

In order to run geo, unzip and untar. If you are lucky, you
can type `./geo < testexamples/blz202_4.geo` and you see that geo finds a proof.

Otherwise, type  `touch Makefile`, type `make` and hope that
the resulting executable works. You need a reasonably
new version of g++, because Geo uses C++11.

Geo accepts the following parameters:

-  `-inputfile %f` Instead of reading from standard input, read from the
   indicated file `%f`.
   
-  `-nonempty`  Do not allow empty models. Without this flag, geo cannot prove
    `forall x. p(x) -> exists x. p(x)`, because the empty model
     is a counter model.
    
-  `-tptp_input` Expect input in TPTP-format.

-  `-include %p` Use `%p` as the path, relative to which include files are defined. TPTP-syntax allows includes. 


## Matching, Constraint Solving

Since geometric resolution relies heavily on constraint solving,
the constraint solver is currently the most sophisticated part of Geo III.
The implementation is probably efficient enough for stand-alone use,
outside of geometric resolution. In order to make this possible,
the constraint solver can be download independently. 
The implementation is in portable C++(11).
The solver reads input from a specified file, and prints output into stdout, either
`UNSAT`, or `SAT` and a satisfying substitution. It can be called with 
option `-cnf`, which will cause it to transform the problem to CNF (Dimacs format)
without trying to solve it.

The input format is similar
to DIMACS format for first-order logic, it is described in Section 7 of 
[this article](GCSP.pdf), which also contains a description of the matching
algorithm used.

[These](geo2018gcsp.tar.gz) are the sources.

In order to run the solver, unzip and untar. If you are lucky, you
can type `./solver gcsp_examples/summer2016/demod06.dim` and watch the solver find
an interpretation.

Otherwise, type  `touch Makefile`, type `make` and hope that
the resulting executable works. You need a reasonably
new version of g++, because the solver uses C++-2014.
Subdirectory `gcsp_examples` contains examples. 

The following input formats are possible

- `./solver` Reads input from stdin, and writes a solution or 'UNSAT' to stdout. 

- `./solver %filename` Reads input from filename, and writes a solution or 'UNSAT' to stdout.

- `./solver -cnf` Reads input from stdin, and writes conversion to CNF to stdout. 
    
- `./solver -cnf %inputfile` Reads input from `%filename` and writes CNF-conversion to stdout.
   The following should work: `./solver -cnf gcsp_examples/summer2016/demod06.dim | minisat`, if you have `minisat` installed.


