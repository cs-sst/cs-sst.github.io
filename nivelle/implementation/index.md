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
can type './geo < blz202_4.geo' and you see that geo finds a proof.

Otherwise, type  'touch Makefile', type 'make' and hope that
the resulting executable works. You need a reasonably
new version of g++, because Geo uses C++11.

Geo accepts the following parameters:
-    -inputfile %f. 
<dd> Instead of reading from standard input, read from the
   indicated file %f.
<dt> -nonempty. 
<dd> Do not allow empty models. Without this flag, geo cannot prove
    forall x. p(x) -> exists x. p(x), because the empty model
    is a counter model.
<dt> -tptp_input. Expect input in TPTP-format. 
-  -include %p
   
Use %p as the path, relative to which include files are defined.
TPTP-syntax allows includes. 



## Matching, Constraint Solver 

Since geometric resolution relies heavily on constraint solving,
the constraint solver is currently the most sophisticated part of Geo III.
The implementation is probably efficient enough for independent use,
outside of geometric resolution. In order to make such applications possible,
we publish the constraint solver as standalone package. 
The implementation is in portable C++(11).
The solver reads input from stdin, and prints outpout into stdout, either
UNSAT, or SAT and a satisfying substitution. 

The input format is similar
to DIMACS format for first-order logic, it is described in Section 7 of 
[this article](GCSP.pdf), which also describes a description of the matching
algorithm used.

<a href = "solver.tar.gz">These</a> are the sources.

There are different benchmark sets.




